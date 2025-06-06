<head>
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
        .pf-certification-list {
            margin-top: 2rem;
            padding-left: 2rem;
        }
        .pf-certification-item {
            margin-bottom: 1rem;
            position: relative;
        }
        .pf-certification-item::before {
            content: "▹";
            position: absolute;
            left: -1.5rem;
            color: #999;
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
        @media (max-width: 768px) {
            .pf-menu-list {
                flex-direction: column;
                align-items: center;
                gap: 1rem;
            }
            .pf-section {
                padding: 2rem 0;
            }
        }
    </style>
</head>
<body>
    <header class="pf-header">
        <div class="pf-container">
            <img src="./static/img/Viter_img.jpeg" alt="Foto profesional" class="pf-header-image">
            <h1>Viter Alonso Rodriguez Quispe</h1>
            <h1>Estudiante Ingeniería de Sistemas</h1>
            <p>Experiencia en Ayuda en Soporte Técnico de Audio y Video en TAM</p>
        </div>
    </header>
    <main class="pf-container">
        <section id="experiencia" class="pf-section">
            <h2 class="pf-section-title">Trayectoria Profesional</h2>
            <div class="pf-experience-content">
                <h3 style="color: #fff; margin-bottom: 1rem; font-size: 1.2rem;">Formación Académica</h3>
                <ul class="pf-certification-list">
                    <li class="pf-certification-item">
                        Ingeniería de Sistemas - Universidad Continental
                    </li>
                </ul>
                <h3 style="color: #fff; margin: 1rem 0; font-size: 1.2rem;">Experiencia Laboral</h3>
                <ul class="pf-certification-list">
                    <li class="pf-certification-item">
                        Ayuda en Soporte Técnico de Audio y Video - TAM
                    </li>
                </ul>
            </div>
        </section>
        <section id="habilidades" class="pf-section">
            <h2 class="pf-section-title">Competencias Técnicas</h2>
            <div class="pf-skills-grid">
                <div class="pf-skill-item">Soporte Técnico</div>
                <div class="pf-skill-item">Audio y Video</div>
                <div class="pf-skill-item">Gestión de Sistemas</div>
                <div class="pf-skill-item">Resolución de Incidencias</div>
                <div class="pf-skill-item">Atención al Cliente</div>
            </div>
        </section>
        <section id="contacto" class="pf-section">
            <h2 class="pf-section-title">Contacto</h2>
            <div class="pf-contact-info">
                <p>📧 75096455@continental.edu.pe</p>
                <p style="margin-top: 1rem;">✆ +51 970404271</p>
            </div>
        </section>
    </main>
</body>
</body>
</html>