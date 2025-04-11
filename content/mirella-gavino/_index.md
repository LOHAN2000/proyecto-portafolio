<link rel="stylesheet" href="../mirella-gavino/css/custom-mirella.css">
<style>
  /* Paleta de colores pastel mejorada */
  :root {
    --fondo-principal: #FFF9FB;
    --fondo-secundario: #FFFFFF;
    --rosa-pastel: #FFD6E0;
    --lila-pastel: #E1C6FF;
    --menta-pastel: #C1F0D0;
    --azul-pastel: #C6E2FF;
    --melocoton-pastel: #FFD8B8;
    --texto-oscuro: #4A4A4A;
    --texto-medio: #6D6D6D;
    --texto-claro: #FFFFFF;
    --acento: #B399D4;
  }
  /* Estilos generales */
  body {
    background-color: var(--fondo-principal);
    color: var(--texto-oscuro);
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 0;
  }
  .custom-container {
    background-color: var(--fondo-secundario);
    box-shadow: 0 0 20px rgba(0,0,0,0.05);
    margin: 20px auto;
    border-radius: 15px;
    overflow: hidden;
  }
  .site-main-wrapper {
    padding: 20px;
  }
  /* Encabezado */
  header {
    background: linear-gradient(135deg, var(--rosa-pastel) 0%, var(--lila-pastel) 100%);
    padding: 2rem 0;
    color: var(--texto-oscuro);
  }
  /* Títulos */
  h1, h2, h3, h4, h5, h6 {
    color: #6E5B7B;
    font-weight: 600;
  }
  h1 {
    font-size: 2.5rem;
    margin-bottom: 1rem;
  }
  h1 span, .section-heading span {
    color: #8B7B96;
  }
  h2 {
    font-size: 1.8rem;
    margin: 1.5rem 0 1rem;
  }
  h3 {
    font-size: 1.4rem;
    color: var(--texto-medio);
  }
  h6 {
    color: var(--acento);
    font-size: 1.1rem;
    margin-bottom: 0.5rem;
  }
  /* Secciones */
  section {
    padding: 3rem 0;
    border-bottom: 1px solid rgba(0,0,0,0.05);
  }
  .about {
    background-color: var(--menta-pastel);
  }
  .services {
    background-color: var(--lila-pastel);
  }
  .freelancer {
    background: linear-gradient(135deg, var(--melocoton-pastel) 0%, var(--rosa-pastel) 100%);
    text-align: center;
    padding: 4rem 0;
  }
  .reviews {
    background-color: var(--azul-pastel);
  }
  .work {
    background-color: #F0F8FF;
  }
  .blog {
    background-color: #FFF0F5;
  }
  .contact {
    background-color: var(--lila-pastel);
    border-bottom: none;
  }
  /* Texto */
  p {
    color: var(--texto-medio);
    font-size: 1.1rem;
    line-height: 1.8;
    margin-bottom: 1.5rem;
  }
  /* Navegación */
  nav {
    padding: 1rem 0;
  }
  nav a {
    color: var(--texto-oscuro);
    text-decoration: none;
    margin-right: 1.5rem;
    font-weight: 500;
    transition: color 0.3s ease;
    font-size: 1.1rem;
  }
  nav a:hover {
    color: var(--acento);
  }
  /* Botones */
  .btn {
    border: none;
    border-radius: 30px;
    padding: 0.8rem 2rem;
    font-weight: 600;
    font-size: 1rem;
    cursor: pointer;
    transition: all 0.3s ease;
    text-transform: uppercase;
    letter-spacing: 1px;
  }
  .btn-primary {
    background-color: var(--acento);
    color: white;
    box-shadow: 0 4px 8px rgba(0,0,0,0.1);
  }
  .btn-primary:hover {
    background-color: #9F86C0;
    transform: translateY(-2px);
  }
  .btn-secondary {
    background-color: var(--menta-pastel);
    color: var(--texto-oscuro);
    border: 2px solid var(--texto-oscuro);
  }
  .btn-secondary:hover {
    background-color: #B5EAD7;
    border-color: var(--acento);
    color: var(--acento);
  }
  /* Tarjetas */
  .card {
    background-color: white;
    border-radius: 12px;
    box-shadow: 0 4px 15px rgba(0,0,0,0.08);
    transition: all 0.3s ease;
    overflow: hidden;
    margin-bottom: 2rem;
  }
  .card:hover {
    transform: translateY(-10px);
    box-shadow: 0 8px 25px rgba(0,0,0,0.12);
  }
  .card img {
    width: 100%;
    height: auto;
    border-bottom: 1px solid rgba(0,0,0,0.05);
  }
  .card-content {
    padding: 1.5rem;
  }
  /* Overlay */
  .overlay {
    background-color: rgba(179, 153, 212, 0.85);
    color: white;
    padding: 1rem;
    text-align: center;
  }
  .overlay span {
    display: block;
    font-size: 0.9rem;
    margin-bottom: 0.5rem;
  }
  .overlay a {
    color: white;
    font-weight: 600;
    text-decoration: none;
  }
  /* Social */
  .social {
    margin-top: 2rem;
  }
  .social a {
    margin-right: 1rem;
    display: inline-block;
    transition: transform 0.3s ease;
  }
  .social a:hover {
    transform: scale(1.1);
  }
  .social img {
    width: 40px;
    height: 40px;
  }
  /* Mobile Nav */
  .mobile-nav {
    background-color: rgba(255, 255, 255, 0.98);
  }
  .mobile-nav ul li a {
    color: var(--texto-oscuro);
  }
  /* Hero Section */
  .hero {
    padding: 3rem 0;
  }
  /* Responsive */
  @media (max-width: 768px) {
    h1 {
      font-size: 2rem;
    }
    .btn {
      padding: 0.7rem 1.5rem;
    }
  }
</style>
<style>
  /* ... (conserva todos los estilos anteriores) ... */
  /* Específicos para la sección de servicios */
  .services .card-wrapper {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 2rem;
    margin-top: 2rem;
  }
  .services .card {
    width: 300px; /* Ancho fijo para las tarjetas */
    text-align: center;
  }
  .services .card img {
    width: 120px; /* Tamaño reducido para las imágenes */
    height: 120px;
    object-fit: contain;
    margin: 1.5rem auto;
    display: block;
    border-bottom: none !important;
  }
  .services .card h2 {
    color: var(--acento);
    margin: 1rem 0;
    font-size: 1.4rem;
  }
  .services .card p {
    padding: 0 1.5rem;
    margin-bottom: 1.5rem;
    font-size: 1rem;
  }
  /* Ajustes para móviles */
  @media (max-width: 768px) {
    .services .card {
      width: 100%;
      max-width: 300px;
    }
    .services .card-wrapper {
      gap: 1.5rem;
    }
  }
</style>

<!-- [El resto del código HTML permanece exactamente igual] -->

<div class="custom-container" style="width: 90%;"> 
  <body>
    <div class="site-main-wrapper" style="width: 90%">
      <button class="hamberger">
        <img src="../mirella-gavino/static/img/hamberger.svg" alt="">
      </button>     
      <div class="mobile-nav">
        <button class="times">
          <img src="../mirella-gavino/static/img/times.svg" alt="">
        </button>
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Services</a></li>
          <li><a href="#">Work</a></li>
          <li><a href="#">Blog</a></li>
        </ul>
      </div>
      <header>
        <div class="container">
          <nav id="main-nav" class="flex items-center justify-between">
            <div class="left flex items-center">
              <div class="branding">
                <img src="../mirella-gavino/static/img/logo3.png" alt="">
              </div>
              <div>
                <a href="#">Inicio</a>
                <a href="#about">Sobre mi</a>
                <a href="#services">Servicios</a>
                <a href="#work">Trabajo</a>
                <a href="#blog">Blog</a>
              </div>
            </div>
            <div class="right">
              <button class="btn btn-primary">Contact</button>
            </div>
          </nav>        
          <div class="hero flex items-center justify-between">
            <div class="left flex-1 flex justify-center">
              <img src="../mirella-gavino/static/img/perfil2.0.png" alt="">
            </div>
            <div class="right flex-1">
              <h6>Mirella Gavino</h6>
              <h1>Soy una Estudiante <span>de Sistemas</span></h1>
              <p>
                Me apasiona la tecnología y la innovación,
                y estoy en constante aprendizaje para combinar
                mis conocimientos técnicos con una orientación al usuario.
              </p>
              <div>
                <button class="btn btn-secondary">DOWNLOAD CV</button>
              </div>
            </div>
          </div>
        </div>
      </header>
      <section id="about" class="about">
        <div class="container flex items-center about-inner-wrap">
          <div class="flex-1">
            <img class="about-me-img" src="../mirella-gavino/static/img/perfil3.0.png" alt="">
          </div>
          <div class="flex-1 right">
            <h1>Sobre <span>Mi</span></h1>
            <h3>Hola! Yo soy Mirella Gavino.</h3>
            <p>
              Soy estudiante de Ingeniería de Sistemas con una sólida trayectoria laboral desde los 17 años en diversos sectores. 
              He trabajado como profesora de matemáticas, en atención al cliente, como cajera y actualmente en el área de desarrollo 
              de clientes. A lo largo de mi experiencia, he desarrollado habilidades en resolución de problemas, comunicación efectiva 
              y gestión de clientes, combinando mi formación en tecnología con un enfoque centrado en el usuario. Estoy en constante 
              aprendizaje y busco aplicar mis conocimientos en entornos dinámicos donde pueda aportar soluciones innovadoras.
            </p>
            <div class="social">
              <a href="#"><img src="../mirella-gavino/static/img/website.png" alt=""></a>
              <a href="https://www.facebook.com/share/15zjTfenLi/?mibextid=wwXIfr"><img src="../mirella-gavino/static/img/fb.png" alt=""></a>
              <a href="https://x.com/thenilskue?s=21"><img src="../mirella-gavino/static/img/x.png" alt=""></a>
              <a href="https://www.instagram.com/nilss.kuesel?igsh=dDV4d2ZnMXBubWxm&utm_source=qr"><img src="../mirella-gavino/static/img/ig.png" alt=""></a>
            </div>
          </div>
        </div>
      </section>
      <section id="services" class="services">
        <div class="container">
          <h1 class="section-heading"><span>Mis </span>Servicios</h1>
          <p>
            Ofrezco servicios de docencia en matemáticas, Elo Boosting en videojuegos competitivos y atención al cliente, 
            garantizando calidad, eficiencia y un enfoque personalizado.
          </p>          
          <div class="card-wrapper">
            <div class="card">
              <img src="../mirella-gavino/static/img/prof.png" alt="">
              <h2>Clases Particulares</h2>
              <p>Adaptación del contenido y metodología según el nivel y necesidades del estudiante.</p>
            </div>           
            <div class="card">
              <img src="../mirella-gavino/static/img/bost.png" alt="">
              <h2>Eloboosting</h2>
              <p>Uso de métodos seguros y sin comprometer la privacidad del jugador.</p>
            </div>          
            <div class="card">
              <img src="../mirella-gavino/static/img/atc.png" alt="">
              <h2>Atencion al Cliente</h2>
              <p>Identificación de oportunidades para aumentar la satisfacción y retención de clientes.</p>
            </div>  
          </div>
        </div>
      </section>
      <section class="freelancer">
        <h1>Mi enfoque es ofrecer un servicio profesional.</h1>
        <p>Disponibilidad y compromiso para brindar la mejor atención.</p>
        <button class="btn btn-primary">Download CV</button>
      </section>
      <section class="reviews">
        <div class="container">
          <h1 class="section-heading"><span>Mi</span> Presentacion</h1>
          <p>Enfocada en la satisfacción y fidelización del usuario.</p>        
          <div class="slider">
            <div class="slide">
              <img src="../mirella-gavino/static/img/perfil4.0.png" alt="">
              <p>
                "Soy una estudiante versátil, con experiencia en atención al cliente, manejo de caja y docencia particular. 
                Combino precisión y organización con un trato cercano y eficiente, adaptándome a cada entorno con compromiso 
                y profesionalismo. Mi objetivo es ofrecer soluciones efectivas, mejorar la experiencia del usuario y seguir 
                creciendo en cada desafío."
              </p>
              <span>- Mirella Gavino</span>
            </div>
          </div>
          <div class="slider-dots"></div>
        </div>
      </section>
      <section id="work" class="work">
        <div class="container">
          <h1 class="section-heading"><span>Mis</span> Empleos</h1>
          <p>Me he desarrolado en distintos sectores a traves de estos 10 años</p>         
          <div class="card-wrapper">
            <div class="card">
              <div class="overlay">
                <span>Categoria</span>
                <a href="#">Desarollo de Cliente</a>
              </div>
              <img src="../mirella-gavino/static/img/makro.png" alt="">
            </div>           
            <div class="card">
              <div class="overlay">
                <span>Categoria</span>
                <a href="#">Atencion al Cliente</a>
              </div>
              <img src="../mirella-gavino/static/img/leña.png" alt="">
            </div>           
            <div class="card">
              <div class="overlay">
                <span>Categoria</span>
                <a href="#">Eloboosting</a>
              </div>
              <img src="../mirella-gavino/static/img/bost.png" alt="">
            </div>            
            <div class="card">
              <div class="overlay">
                <span>Categoria</span>
                <a href="#">Docencia Particular</a>
              </div>
              <img src="../mirella-gavino/static/img/docent.png" alt="">
            </div> 
            <div class="card">
              <div class="overlay">
                <span>Categoria</span>
                <a href="#">Atencion al cliente</a>
              </div>
              <img src="../mirella-gavino/static/img/mdy.png" alt="">
            </div>           
            <div class="card">
              <div class="overlay">
                <span>Categoria</span>
                <a href="#">Atencion al Cliente</a>
              </div>
              <img src="../mirella-gavino/static/img/gmg.png" alt="">
            </div>
          </div>
        </div>
      </section>
      <section id="blog" class="blog">
        <div class="container">
          <h1 class="section-heading"><span>Mi</span> Blog</h1>
          <p>
            Desde los 17 años, he construido una trayectoria laboral diversa que me ha permitido desarrollar habilidades 
            en múltiples áreas. Mi experiencia abarca desde la enseñanza particular hasta la atención al cliente y el desarrollo 
            de clientes, cada una aportando valiosas lecciones que han enriquecido mi perfil profesional. A lo largo de los años, 
            he aprendido a adaptarme a distintos entornos, comprender las necesidades de las personas y ofrecer soluciones efectivas.
          </p> 
          <div class="card-wrapper">
            <div class="card">
              <div class="img-wrapper">
                <img src="../mirella-gavino/static/img/12323.jpg" alt="">
              </div>
              <div class="card-content">
                <a href="#">
                  <h1>La pasión por enseñar</h1>
                </a>
                <span>Enero 18, 2015</span>
                <p>
                  Uno de mis primeros pasos en el mundo laboral fue la docencia particular en matemáticas. Brindar apoyo a estudiantes 
                  me permitió desarrollar habilidades pedagógicas, paciencia y la capacidad de adaptar mis métodos de enseñanza a diferentes 
                  estilos de aprendizaje. Aprendí a comunicar ideas complejas de manera clara y efectiva, lo que me ha resultado útil en 
                  todas las áreas en las que he trabajado.
                </p>
              </div>
            </div>   
            <div class="card">
              <div class="img-wrapper">
                <img src="../mirella-gavino/static/img/c1234.jpg" alt="">
              </div>
              <div class="card-content">
                <a href="#">
                  <h1>La clave de la comunicación y organizacion</h1>
                </a>
                <span>Agosto 18, 2016</span>
                <p>
                  Trabajar en atención al cliente y como cajera me dio una perspectiva única sobre la importancia del servicio y la eficiencia 
                  operativa. Desarrollé habilidades en resolución de problemas, gestión de tiempo y comunicación efectiva. Aprendí a manejar 
                  situaciones bajo presión, a brindar un trato amable y a garantizar una experiencia satisfactoria para cada cliente. Esta 
                  experiencia me enseñó la importancia de la empatía y la capacidad de respuesta rápida.
                </p>
              </div>
            </div>   
            <div class="card">
              <div class="img-wrapper">
                <img src="../mirella-gavino/static/img/asdd45.jpg" alt="">
              </div>
              <div class="card-content">
                <a href="#">
                  <h1>Conectando necesidades con soluciones</h1>
                </a>
                <span>Febrero 03, 2025</span>
                <p>
                  Actualmente, mi enfoque está en el desarrollo de clientes, donde combino mis habilidades en comunicación y resolución de 
                  problemas para crear relaciones sólidas con los clientes. Mi capacidad de análisis y comprensión de las necesidades del 
                  usuario me permite identificar oportunidades de mejora y crecimiento. En este rol, aplico tanto mis conocimientos técnicos 
                  como mi experiencia en atención al cliente para ofrecer soluciones efectivas y generar valor para cada cliente con el que trabajo.
                </p>
              </div>
            </div>
          </div>
        </div>
      </section>
      <section class="contact">
        <div class="container">
          <h1 class="section-heading">Contactame <span>Aqui</span></h1>
          <p>
            Si buscas una profesional versátil con experiencia en docencia, atención al cliente y desarrollo de clientes, 
            contáctame para colaborar juntos
          </p>    
          <div class="card-wrapper">
            <div class="card">
              <img src="../mirella-gavino/static/img/phone.jpg.png" alt="">
              <h1>Llama al</h1>
              <h6>+51 900661827</h6>
            </div>      
            <div class="card">
              <img src="../mirella-gavino/static/img/gmail.jpg" alt="">
              <h1>Email</h1>
              <h6>mgavino614@gmail.com</h6>
            </div>    
            <div class="card">
              <img src="../mirella-gavino/static/img/wspp.jpg.png" alt="">
              <h1>WhatsApp</h1>
              <h6>+51 926661827</h6>
            </div>
          </div>
        </div>
      </section>
    </div>
  </body>
</div>