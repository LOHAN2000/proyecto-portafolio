<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gerardo Campos - Portafolio</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', system-ui, sans-serif;
        }
        body {
            background-color: #000;
            color: #fff;
        }
        .pf-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        .pf-header {
            background: #000;
            color: #fff;
            padding: 4rem 0;
            text-align: center;
        }
        .pf-header-image {
            width: 250px;
            height: 250px;
            border-radius: 50%;
            object-fit: cover;
            margin-bottom: 1.5rem;
            border: 4px solid #fff;
        }
        .pf-main-menu {
            background: #222;
            padding: 1.2rem 0;
            position: sticky;
            top: 0;
            z-index: 100;
        }
        .pf-menu-list {
            list-style: none;
            display: flex;
            justify-content: center;
            gap: 2rem;
        }
        .pf-menu-link {
            color: #fff;
            text-decoration: none;
            font-weight: 500;
            transition: opacity 0.3s;
        }
        .pf-menu-link:hover {
            opacity: 0.8;
        }
        .pf-section {
            padding: 4rem 0;
            border-bottom: 1px solid #333;
        }
        .pf-section-title {
            font-size: 2rem;
            margin-bottom: 2rem;
            color: #fff;
            text-transform: uppercase;
            letter-spacing: 2px;
        }
        .pf-experience-content {
            background: #1a1a1a;
            padding: 2rem;
            margin-bottom: 2rem;
            border: 1px solid #333;
        }
        .pf-skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 1rem;
            margin-top: 1.5rem;
        }
        .pf-skill-item {
            background: #1a1a1a;
            padding: 1.2rem;
            text-align: center;
            border: 1px solid #333;
            transition: transform 0.3s;
            color: #fff;
        }
        .pf-skill-item:hover {
            transform: translateY(-3px);
        }
        .pf-contact-info {
            background: #111;
            padding: 2rem;
            margin-top: 2rem;
        }
        .pf-footer {
            background: #000;
            color: #fff;
            text-align: center;
            padding: 2rem 0;
            margin-top: 4rem;
        }
        /* Nuevos estilos para la sección de experiencia */
        .pf-exp-subsection {
            background: #1a1a1a;
            padding: 2rem;
            margin-bottom: 2rem;
            border-left: 4px solid #00ff88;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .pf-exp-subsection:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(0, 255, 136, 0.1);
        }
        .pf-subsection-header {
            display: flex;
            align-items: center;
            margin-bottom: 1.5rem;
        }
        .pf-subsection-icon {
            width: 32px;
            height: 32px;
            margin-right: 1rem;
            color: #00ff88;
        }
        .pf-subsection-title {
            font-size: 1.4rem;
            color: #00ff88;
            text-transform: uppercase;
            letter-spacing: 1px;
        }
        .pf-timeline-item {
            display: flex;
            position: relative;
            padding-left: 30px;
            margin-bottom: 2rem;
        }
        .pf-timeline-marker {
            position: absolute;
            left: 0;
            top: 5px;
            width: 16px;
            height: 16px;
            background: #00ff88;
            border-radius: 50%;
        }
        .pf-timeline-content {
            flex: 1;
        }
        .pf-timeline-duration {
            color: #888;
            font-size: 0.9rem;
            margin: 0.3rem 0;
        }
        .pf-university {
            color: #00ff88;
            font-weight: 500;
        }
        .pf-highlight-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1.5rem;
        }
        .pf-highlight-card {
            background: #252525;
            padding: 1.5rem;
            text-align: center;
            border-radius: 8px;
        }
        .pf-card-number {
            font-size: 2.5rem;
            font-weight: 700;
            color: #00ff88;
            margin-bottom: 0.5rem;
        }
        .pf-specialization-grid {
            display: grid;
            gap: 1.5rem;
        }
        .pf-specialty-item {
            display: flex;
            align-items: center;
            background: #252525;
            padding: 1.5rem;
            border-radius: 8px;
        }
        .pf-specialty-icon {
            font-size: 1.5rem;
            margin-right: 1rem;
            color: #00ff88;
        }
        @media (max-width: 768px) {
            .pf-menu-list {
                flex-direction: column;
                align-items: center;
                gap: 1rem;
            }
            .pf-section {
                padding: 2rem 0;
            }
            .pf-exp-subsection {
                padding: 1.5rem;
            }
            .pf-subsection-title {
                font-size: 1.2rem;
            }
        }
        .pf-skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 1.5rem;
            margin-top: 2rem;
        }
        .pf-skill-item {
            background: #1a1a1a;
            padding: 1.5rem;
            border-radius: 8px;
            border: 1px solid #333;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }
        .pf-skill-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0, 255, 136, 0.15);
            border-color: #00ff88;
        }
        .pf-skill-item::before {
            content: "▹";
            position: absolute;
            left: 1rem;
            color: #00ff88;
            font-size: 1.2rem;
        }
        /* Nuevos estilos para Contacto */
        .pf-contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }
        .pf-contact-card {
            background: #1a1a1a;
            padding: 2rem;
            border-radius: 10px;
            border: 1px solid #333;
            transition: all 0.3s ease;
            text-align: center;
        }
        .pf-contact-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0, 255, 136, 0.15);
        }
        .pf-contact-icon {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: #00ff88;
        }
        .pf-contact-details {
            margin-top: 1.5rem;
        }
        .pf-contact-details p {
            margin: 0.5rem 0;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 0.5rem;
        }
        @media (max-width: 768px) {
            .pf-skill-item {
                padding: 1.2rem;
            }
            .pf-contact-card {
                padding: 1.5rem;
            }
        }
    </style>
</head>
<body>
    <header class="pf-header">
        <div class="pf-container">
            <img src="./static/img/gerardo.jpeg" alt="Foto profesional" class="pf-header-image">
            <h1>Gerardo Campos Velasquez</h1>
            <h1>Especialista en Infraestructura TI</h1>
            <p>Más de 10 años liderando proyectos tecnológicos en retail</p>
        </div>
    </header>
    <main class="pf-container">
        <section id="experiencia" class="pf-section">
            <h2 class="pf-section-title">Trayectoria Profesional</h2>
            <div class="pf-experience-content">
                <div class="pf-exp-subsection">
                    <div class="pf-subsection-header">
                        <svg class="pf-subsection-icon" viewBox="0 0 24 24" width="24" height="24">
                            <path fill="currentColor" d="M12 3L1 9l4 2.18v6L12 21l7-3.82v-6l2-1.09V17h2V9L12 3m6.82 6L12 12.72L5.18 9L12 5.28L18.82 9M17 16l-5 2.72L7 16v-3.73L12 15l5-2.73V16Z"/>
                        </svg>
                        <h3 class="pf-subsection-title">Formación Académica</h3>
                    </div>
                    <div class="pf-timeline-item">
                        <div class="pf-timeline-marker"></div>
                        <div class="pf-timeline-content">
                            <h4>Ingeniería de Sistemas</h4>
                            <p class="pf-timeline-duration">2022 - Actualidad</p>
                            <p class="pf-university">Universidad Continental</p>
                        </div>
                    </div>
                </div>
                <div class="pf-exp-subsection">
                    <div class="pf-subsection-header">
                        <svg class="pf-subsection-icon" viewBox="0 0 24 24" width="24" height="24">
                            <path fill="currentColor" d="M18 15v3H6v-3H4v3c0 1.1.9 2 2 2h12c1.1 0 2-.9 2-2v-3h-2zm-1-4l-1.41-1.41L13 12.17V4h-2v8.17L8.41 9.59L7 11l5 5l5-5z"/>
                        </svg>
                        <h3 class="pf-subsection-title">Logros Clave</h3>
                    </div>
                    <div class="pf-highlight-grid">
                        <div class="pf-highlight-card">
                            <div class="pf-card-number">5+</div>
                            <h4>Años de Experiencia</h4>
                            <p>Sector Retail</p>
                        </div>
                        <div class="pf-highlight-card">
                            <div class="pf-card-number">50+</div>
                            <h4>Proyectos Liderados</h4>
                            <p>Implementados con éxito</p>
                        </div>
                    </div>
                </div>
                <div class="pf-exp-subsection">
                    <div class="pf-subsection-header">
                        <svg class="pf-subsection-icon" viewBox="0 0 24 24" width="24" height="24">
                            <path fill="currentColor" d="M12 1L3 5v6c0 5.55 3.84 10.74 9 12c5.16-1.26 9-6.45 9-12V5l-9-4zm0 10.99h7c-.53 4.12-3.28 7.79-7 8.94V12H5V6.3l7-3.11v8.8z"/>
                        </svg>
                        <h3 class="pf-subsection-title">Especializaciones</h3>
                    </div>
                    <div class="pf-specialization-grid">
                        <div class="pf-specialty-item">
                            <div class="pf-specialty-icon">✓</div>
                            <div class="pf-specialty-content">
                                <h4>Infraestructuras Críticas</h4>
                                <p>Gestión de sistemas 24/7 para operaciones continuas</p>
                            </div>
                        </div>
                        <div class="pf-specialty-item">
                            <div class="pf-specialty-icon">✓</div>
                            <div class="pf-specialty-content">
                                <h4>Transformación Digital</h4>
                                <p>Modernización de procesos empresariales</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        <section id="habilidades" class="pf-section">
        <h2 class="pf-section-title">Competencias Técnicas</h2>
        <div class="pf-skills-grid">
            <div class="pf-skill-item">
                Gestión de Servicios TI
                <div class="pf-skill-progress">
                    <div class="pf-progress-bar" style="width: 95%"></div>
                </div>
            </div>
            <div class="pf-skill-item">
                Infraestructura Cloud
                <div class="pf-skill-progress">
                    <div class="pf-progress-bar" style="width: 85%"></div>
                </div>
            </div>
            <div class="pf-skill-item">
                Seguridad de Sistemas
                <div class="pf-skill-progress">
                    <div class="pf-progress-bar" style="width: 90%"></div>
                </div>
            </div>
            <div class="pf-skill-item">
                Gestión de Proyectos
                <div class="pf-skill-progress">
                    <div class="pf-progress-bar" style="width: 88%"></div>
                </div>
            </div>
            <div class="pf-skill-item">
                Service Desk Enterprise
                <div class="pf-skill-progress">
                    <div class="pf-progress-bar" style="width: 92%"></div>
                </div>
            </div>
        </div>
    </section>
    <section id="contacto" class="pf-section">
        <h2 class="pf-section-title">Contacto</h2>
        <div class="pf-contact-grid">
            <div class="pf-contact-card">
                <div class="pf-contact-icon">📧</div>
                <h3>Correo Electrónico</h3>
                <div class="pf-contact-details">
                    <p>43303380@continental.edu.pe</p>
                </div>
            </div>
            <div class="pf-contact-card">
                <div class="pf-contact-icon">📱</div>
                <h3>Teléfono</h3>
                <div class="pf-contact-details">
                    <p>+51 955751813</p>
                </div>
            </div>
        </div>
    </section>
    </main>
</body>
</html>