<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Andrea Clemente-Ureña - Portfolio</title>
  <style>
    :root {
      --primary: #2E7D32;  /* Verde principal */
      --secondary: #388E3C; /* Verde secundario */
      --accent: #43A047;    /* Verde acento */
      --light: #C8E6C9;    /* Verde claro */
      --text: #1B5E20;     /* Verde oscuro para texto */
      --bg: #F1F8E9;       /* Fondo verde claro */
      --card: #FFFFFF;     /* Tarjetas blancas */
    }
    
    body {
      font-family: "Segoe UI", sans-serif;
      margin: 0;
      padding: 2rem;
      line-height: 1.7;
      background-color: var(--bg);
      color: var(--text);
      font-size: 1.2rem;
    }
    
    h1, h2, h3 {
      color: var(--primary);
      font-weight: 600;
    }
    
    a {
      color: var(--secondary);
      text-decoration: none;
      transition: color 0.3s;
    }
    
    a:hover {
      color: var(--accent);
    }
    
    header {
      text-align: center;
      margin-bottom: 3rem;
      padding: 2rem;
      background: linear-gradient(135deg, var(--light) 0%, var(--accent) 100%);
      border-radius: 15px;
      color: white;
    }
    
    header h1 {
      font-size: 2.8rem;
      margin-bottom: 1rem;
      color: white;
    }
    
    header p {
      font-size: 1.4rem;
      margin-bottom: 0.5rem;
      color: white;
    }
    
    .section-title {
      text-align: center;
      margin: 4rem 0 2rem;
      font-size: 2.2rem;
      position: relative;
    }
    
    .section-title:after {
      content: "";
      display: block;
      width: 100px;
      height: 4px;
      background: var(--accent);
      margin: 1rem auto;
      border-radius: 2px;
    }
    
    .direct-section {
      background-color: var(--card);
      padding: 2.5rem;
      border-radius: 15px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.08);
      margin: 3rem 0;
      transition: transform 0.3s, box-shadow 0.3s;
    }
    
    .direct-section:hover {
      transform: translateY(-5px);
      box-shadow: 0 10px 25px rgba(0,0,0,0.12);
    }
    
    /* Proyectos */
    .project-container {
      margin: 4rem 0;
    }
    
    .project-title {
      text-align: center;
      font-size: 1.8rem;
      color: var(--primary);
      margin-bottom: 1.5rem;
      font-weight: 500;
    }
    
    .project-image {
      width: 300px; /* 3 veces más pequeña que 900px */
      margin: 0 auto 2rem;
      border: 8px solid white;
      box-shadow: 0 5px 15px rgba(0,0,0,0.1);
      transition: transform 0.3s;
    }
    
    .project-image:hover {
      transform: scale(1.05);
    }
    
    .project-image img {
      width: 100%;
      display: block;
    }
    
    .project-description {
      max-width: 800px;
      margin: 0 auto;
      font-size: 1.2rem;
      line-height: 1.8;
    }
    
    /* Formación y experiencia */
    .timeline-item {
      position: relative;
      padding-left: 3rem;
      margin-bottom: 2.5rem;
    }
    
    .timeline-item:before {
      content: "";
      position: absolute;
      left: 0;
      top: 5px;
      width: 20px;
      height: 20px;
      border-radius: 50%;
      background: var(--accent);
      border: 4px solid var(--light);
    }
    
    .timeline-item:after {
      content: "";
      position: absolute;
      left: 10px;
      top: 25px;
      bottom: -25px;
      width: 2px;
      background: var(--light);
    }
    
    .timeline-item:last-child:after {
      display: none;
    }
    
    .timeline-date {
      font-weight: 500;
      color: var(--secondary);
    }
    
    /* Tecnologías */
    .skills-category {
      margin-bottom: 2rem;
    }
    
    .skills-category h3 {
      color: var(--secondary);
      margin-bottom: 1rem;
      font-size: 1.4rem;
    }
    
    .skills-list {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }
    
    .skill-tag {
      background: var(--light);
      color: white;
      padding: 5px 15px;
      border-radius: 20px;
      font-size: 1rem;
    }
    
    /* Idiomas */
    .language-item {
      display: flex;
      align-items: center;
      margin-bottom: 1rem;
      font-size: 1.3rem;
    }
    
    .language-flag {
      font-size: 2rem;
      margin-right: 1rem;
    }
    
    /* Contacto */
    #contact-form {
      max-width: 700px;
      margin: 3rem auto;
      background: white;
      padding: 2.5rem;
      border-radius: 15px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.08);
    }
    
    #contact-form label {
      display: block;
      margin: 1.5rem 0 0.5rem;
      color: var(--primary);
      font-weight: 500;
    }
    
    #contact-form input,
    #contact-form textarea {
      width: 100%;
      padding: 12px;
      border: 2px solid #eee;
      border-radius: 8px;
      font-size: 1.1rem;
      transition: border-color 0.3s;
    }
    
    #contact-form input:focus,
    #contact-form textarea:focus {
      border-color: var(--light);
      outline: none;
    }
    
    #contact-form textarea {
      min-height: 150px;
    }
    
    #contact-form input[type="submit"] {
      background: var(--secondary);
      color: white;
      border: none;
      padding: 15px 30px;
      font-size: 1.2rem;
      border-radius: 8px;
      cursor: pointer;
      margin-top: 2rem;
      transition: background 0.3s;
    }
    
    #contact-form input[type="submit"]:hover {
      background: var(--accent);
    }
    
    /* Footer */
    footer {
      text-align: center;
      margin: 4rem 0 2rem;
      font-size: 1.3rem;
      color: var(--text);
      padding: 2rem;
      font-style: italic;
    }
    
    /* Botón de idioma */
    #language-toggle {
      position: fixed;
      top: 20px;
      right: 20px;
      padding: 10px 20px;
      background: var(--primary);
      color: white;
      border: none;
      border-radius: 30px;
      cursor: pointer;
      z-index: 1000;
      font-size: 1.1rem;
      box-shadow: 0 3px 10px rgba(0,0,0,0.2);
      transition: all 0.3s;
    }
    
    #language-toggle:hover {
      background: var(--secondary);
      transform: translateY(-2px);
    }
    
    /* Responsive */
    @media (max-width: 768px) {
      body {
        padding: 1rem;
        font-size: 1.1rem;
      }
      
      header h1 {
        font-size: 2rem;
      }
      
      .section-title {
        font-size: 1.8rem;
      }
      
      .direct-section {
        padding: 1.5rem;
      }
      
      .project-image {
        width: 100%;
      }
    }
  </style>
</head>
<body>

<button id="language-toggle" onclick="toggleLanguage()">English</button>

<header>
  <h1>
    <span class="lang-es">Andrea Clemente-Ureña</span>
    <span class="lang-en">Andrea Clemente-Ureña</span>
  </h1>
  <p>
    <span class="lang-es">Bióloga | Bioinformática | Visión Computacional | IA</span>
    <span class="lang-en">Biologist | Bioinformatics | Computer Vision | AI</span>
  </p>
  <p>
    <span class="lang-es">Investigadora predoctoral en UPM y CRF-INIA-CSIC</span>
    <span class="lang-en">Predoctoral Researcher at UPM and CRF-INIA-CSIC</span>
  </p>
</header>

<!-- Bienvenida -->
<section id="bienvenida" class="direct-section">
  <img class="section-img" src="beautiful-landscape-with-rainbow-plants.jpg" alt="Bienvenida" style="width: 100%; max-width: 900px; margin: 0 auto 2rem; border-radius: 15px;">
  <p style="text-align: center; font-size: 1.4rem;">
    <span class="lang-es">Bienvenid@ a mi portfolio científico</span>
    <span class="lang-en">Welcome to my scientific portfolio</span>
  </p>
  <p>
    <span class="lang-es">Soy una investigadora apasionada por la intersección entre la biología y la tecnología. Mi trabajo se centra en desarrollar herramientas innovadoras para el fenotipado de cultivos y la caracterización de estructuras vegetales mediante visión por computador 3D y aprendizaje automático.</span>
    <span class="lang-en">I'm a researcher passionate about the intersection between biology and technology. My work focuses on developing innovative tools for crop phenotyping and plant structure characterization using 3D computer vision and machine learning.</span>
  </p>
</section>

<!-- Primer contacto con investigación -->
<section id="primer-contacto-section" class="direct-section">
  <h2 class="section-title">
    <span class="lang-es">💡 Primer contacto con la investigación</span>
    <span class="lang-en">💡 First Research Experience</span>
  </h2>
  
  <div class="project-container">
    <div class="project-title">
      <span class="lang-es">Síntesis de bioplásticos</span>
      <span class="lang-en">Bioplastics Synthesis</span>
    </div>
    <div class="project-image">
      <img src="laboratory-samples-arrangement.jpg" alt="Síntesis de bioplásticos">
    </div>
    <div class="project-description">
      <p>
        <span class="lang-es">Proyecto desarrollado en 1º de Bachillerato sobre síntesis de bioplásticos a partir de leche de vaca, combinando conceptos de biología y química.</span>
        <span class="lang-en">High school project about synthesizing bioplastics from cow milk, combining biology and chemistry concepts.</span>
      </p>
    </div>
  </div>
  
  <div class="project-container">
    <div class="project-title">
      <span class="lang-es">Finde Científico</span>
      <span class="lang-en">Science Weekend</span>
    </div>
    <div class="project-image">
      <img src="lab-glassware-with-colored-liquids-assortment.jpg" alt="Finde Científico">
    </div>
    <div class="project-description">
      <p>
        <span class="lang-es">Participación en eventos de divulgación científica realizando experimentos de química visual para acercar la ciencia al público general.</span>
        <span class="lang-en">Participation in science outreach events performing visual chemistry experiments to bring science closer to the general public.</span>
      </p>
    </div>
  </div>
</section>

<!-- Proyectos destacados -->
<section id="proyectos-section" class="direct-section">
  <h2 class="section-title">
    <span class="lang-es">🚀 Proyectos Destacados</span>
    <span class="lang-en">🚀 Featured Projects</span>
  </h2>
  
  <!-- Proyecto 1 -->
  <div class="project-container">
    <div class="project-title">
      <span class="lang-es">Fenotipado Automatizado</span>
      <span class="lang-en">Automated Phenotyping</span>
    </div>
    <div class="project-image">
      <img src="3461225.jpg" alt="Fenotipado de cultivos">
    </div>
    <div class="project-description">
      <p>
        <span class="lang-es">Desarrollo de sistemas robóticos para fenotipado de alto rendimiento en cultivos, integrando visión por computador y análisis de datos.</span>
        <span class="lang-en">Development of robotic systems for high-throughput crop phenotyping, integrating computer vision and data analysis.</span>
      </p>
    </div>
  </div>
  
  <!-- Proyecto 2 -->
  <div class="project-container">
    <div class="project-title">
      <span class="lang-es">Bioinformática en Huntington</span>
      <span class="lang-en">Huntington's Bioinformatics</span>
    </div>
    <div class="project-image">
      <img src="https://github.com/user-attachments/assets/8dfa2628-f892-4078-bde3-3915150bed34" alt="Bioinformática">
    </div>
    <div class="project-description">
      <p>
        <span class="lang-es">TFM: Identificación y caracterización de tRFs sobreexpresados en enfermedad de Huntington mediante análisis bioinformático.</span>
        <span class="lang-en">Master's Thesis: Identification and characterization of overexpressed tRFs in Huntington's disease through bioinformatics analysis.</span>
      </p>
      <p>
        <span class="lang-es">DOI: <a href="https://doi.org/10.13140/RG.2.2.33680.32001" target="_blank">10.13140/RG.2.2.33680.32001</a></span>
        <span class="lang-en">DOI: <a href="https://doi.org/10.13140/RG.2.2.33680.32001" target="_blank">10.13140/RG.2.2.33680.32001</a></span>
      </p>
    </div>
  </div>
  
  <!-- Proyecto 3 -->
  <div class="project-container">
    <div class="project-title">
      <span class="lang-es">Genética en Leishmania</span>
      <span class="lang-en">Leishmania Genetics</span>
    </div>
    <div class="project-image">
      <img src="https://github.com/user-attachments/assets/b740f460-1160-4a35-90c6-b3b2e5861f23" alt="Genética molecular">
    </div>
    <div class="project-description">
      <p>
        <span class="lang-es">TFG: Caracterización estructural de genes codificantes de proteínas ribosómicas en Leishmania.</span>
        <span class="lang-en">Bachelor's Thesis: Structural characterization of genes coding for ribosomal proteins in Leishmania.</span>
      </p>
      <p>
        <span class="lang-es">DOI: <a href="https://doi.org/10.13140/RG.2.2.10192.21767" target="_blank">10.13140/RG.2.2.10192.21767</a></span>
        <span class="lang-en">DOI: <a href="https://doi.org/10.13140/RG.2.2.10192.21767" target="_blank">10.13140/RG.2.2.10192.21767</a></span>
      </p>
    </div>
  </div>
</section>

<!-- Formación académica -->
<section id="formacion-section" class="direct-section">
  <h2 class="section-title">
    <span class="lang-es">🎓 Formación Académica</span>
    <span class="lang-en">🎓 Academic Education</span>
  </h2>
  
  <div class="timeline-item">
    <div class="timeline-date">2024 - Presente</div>
    <h3>
      <span class="lang-es">Doctorado en Automática y Robótica</span>
      <span class="lang-en">PhD in Automation and Robotics</span>
    </h3>
    <p>Universidad Politécnica de Madrid – INIA-CSIC</p>
  </div>
  
  <div class="timeline-item">
    <div class="timeline-date">2022 - 2024</div>
    <h3>
      <span class="lang-es">Máster en Bioinformática y Bioestadística</span>
      <span class="lang-en">Master in Bioinformatics and Biostatistics</span>
    </h3>
    <p>Universitat Oberta de Catalunya / Universitat de Barcelona</p>
 
  </div>
  
  <div class="timeline-item">
    <div class="timeline-date">2016 - 2021</div>
    <h3>
      <span class="lang-es">Grado en Biología</span>
      <span class="lang-en">Bachelor in Biology</span>
    </h3>
    <p>Universidad Autónoma de Madrid</p>
    <p>Especialidad en Biología Molecular y Genética</p>
  </div>
  
  <div class="timeline-item">
    <div class="timeline-date">2014 - 2016</div>
    <h3>
      <span class="lang-es">Técnico Superior en Anatomía Patológica y citología</span>
      <span class="lang-en">Higher Technician in Pathological Anatomy and Citology</span>
    </h3>
    <p>CESUR II, Madrid</p>
  </div>
</section>

<!-- Habilidades -->
<section id="tecnologias-section" class="direct-section">
  <h2 class="section-title">
    <span class="lang-es">🛠️ Habilidades Técnicas</span>
    <span class="lang-en">🛠️ Technical Skills</span>
  </h2>
  
  <div class="skills-category">
    <h3>
      <span class="lang-es">Lenguajes de Programación</span>
      <span class="lang-en">Programming Languages</span>
    </h3>
    <div class="skills-list">
      <span class="skill-tag">Python</span>
      <span class="skill-tag">R</span>
      <span class="skill-tag">Bash</span>
      <span class="skill-tag">SQL</span>
    </div>
  </div>
  
  <div class="skills-category">
    <h3>
      <span class="lang-es">Bioinformática</span>
      <span class="lang-en">Bioinformatics</span>
    </h3>
    <div class="skills-list">
      <span class="skill-tag">Bioconductor</span>
      <span class="skill-tag">Galaxy</span>
      <span class="skill-tag">NovoPath</span>
      <span class="skill-tag">SPSS</span>
    </div>
  </div>
  
  <div class="skills-category">
    <h3>
      <span class="lang-es">IA & Visión por Computador</span>
      <span class="lang-en">AI & Computer Vision</span>
    </h3>
    <div class="skills-list">
      <span class="skill-tag">PyTorch</span>
      <span class="skill-tag">TensorFlow</span>
      <span class="skill-tag">OpenCV</span>
      <span class="skill-tag">Scikit-learn</span>
    </div>
  </div>
  
  <div class="skills-category">
    <h3>
      <span class="lang-es">Robótica</span>
      <span class="lang-en">Robotics</span>
    </h3>
    <div class="skills-list">
      <span class="skill-tag">HoloLens 2</span>
      <span class="skill-tag">Sensores LiDAR</span>
      <span class="skill-tag">Sensores RGB-D</span>
      <span class="skill-tag">ROS</span>
    </div>
  </div>
</section>

<!-- Experiencia -->
<section id="experiencia-section" class="direct-section">
  <h2 class="section-title">
    <span class="lang-es">💼 Experiencia Profesional</span>
    <span class="lang-en">💼 Professional Experience</span>
  </h2>
  
  <div class="timeline-item">
    <div class="timeline-date">2024 - Presente</div>
    <h3>
      <span class="lang-es">Investigadora Predoctoral</span>
      <span class="lang-en">Predoctoral Researcher</span>
    </h3>
    <p>INIA-CSIC / UPM</p>
    <p>
      <span class="lang-es">Desarrollo de sistemas de visión 3D para fenotipado automatizado de cultivos en el proyecto "Transformación digital de la conservación y mejora vegetal".</span>
      <span class="lang-en">Development of 3D vision systems for automated crop phenotyping in the project "Digital Transformation of Plant Conservation and Improvement".</span>
    </p>
  </div>
  
  <div class="timeline-item">
    <div class="timeline-date">2021</div>
    <h3>
      <span class="lang-es">Teleoperadora Comercial</span>
      <span class="lang-en">Commercial Operator</span>
    </h3>
    <p>My Assessor Total</p>
    <p>
      <span class="lang-es">Atención al cliente y venta telefónica.</span>
      <span class="lang-en">Customer service and telephone sales.</span>
    </p>
  </div>
  
  <div class="timeline-item">
    <div class="timeline-date">2016</div>
    <h3>
      <span class="lang-es">Técnico de Anatomía Patológica</span>
      <span class="lang-en">Pathological Anatomy Technician</span>
    </h3>
    <p>HM Hospitales</p>
    <p>
      <span class="lang-es">Procesamiento de muestras y técnicas histológicas.</span>
      <span class="lang-en">Sample processing and histological techniques.</span>
    </p>
  </div>
</section>

<!-- Idiomas -->
<section id="idiomas-section" class="direct-section">
  <h2 class="section-title">
    <span class="lang-es">🌐 Idiomas</span>
    <span class="lang-en">🌐 Languages</span>
  </h2>
  
  <div class="language-item">
    <span class="language-flag">🇪🇸</span>
    <span>
      <span class="lang-es">Español: Nativo</span>
      <span class="lang-en">Spanish: Native</span>
    </span>
  </div>
  
  <div class="language-item">
    <span class="language-flag">🇬🇧</span>
    <span>
      <span class="lang-es">Inglés: Nivel C (APTIS - British Council)</span>
      <span class="lang-en">English: Level C (APTIS - British Council)</span>
    </span>
  </div>
  
  <div class="language-item">
    <span class="language-flag">🇫🇷</span>
    <span>
      <span class="lang-es">Francés: Nivel A2 (DELF)</span>
      <span class="lang-en">French: Level A2 (DELF)</span>
    </span>
  </div>
</section>

<!-- Contacto -->
<section id="contacto-section" class="direct-section">
  <h2 class="section-title">
    <span class="lang-es">📫 Contacto</span>
    <span class="lang-en">📫 Contact</span>
  </h2>
  
  <div style="text-align: center; font-size: 1.3rem; line-height: 2.5;">
    <div>
      <span class="lang-es">Puedes contactarme a través de:</span>
      <span class="lang-en">You can contact me through:</span>
    </div>
    <div>
      <a href="https://www.researchgate.net/profile/Andrea-Clemente-Urena-2" target="_blank">ResearchGate</a>
    </div>
    <div>
      <a href="https://www.linkedin.com/in/andreaclementeure%C3%B1a/" target="_blank">LinkedIn</a>
    </div>
    <div>
      <a href="https://github.com/andreaclemente96" target="_blank">GitHub</a>
    </div>
  </div>
</section>

<!-- Formulario de contacto -->
<form id="contact-form" action="https://formspree.io/f/andeande.ac@gmail.com" method="POST">
  <h2 class="section-title">
    <span class="lang-es">✉️ Envíame un mensaje</span>
    <span class="lang-en">✉️ Send me a message</span>
  </h2>
  
  <label for="name">
    <span class="lang-es">Nombre</span>
    <span class="lang-en">Name</span>
  </label>
  <input type="text" id="name" name="name" required>
  
  <label for="email">
    <span class="lang-es">Tu email</span>
    <span class="lang-en">Your email</span>
  </label>
  <input type="email" id="email" name="email" required>
  
  <label for="message">
    <span class="lang-es">Mensaje</span>
    <span class="lang-en">Message</span>
  </label>
  <textarea id="message" name="message" required></textarea>
  
  <input type="submit" value="Enviar">
</form>

<footer>
  <p>
    <span class="lang-es">"La IA no es el enemigo, es la lupa que amplifica lo que la ciencia aún no alcanza." 🤖🔬🌍</span>
    <span class="lang-en">"AI is not the enemy; it is the magnifying glass that amplifies what science has not yet reached." 🤖🔬🌍</span>
  </p>
</footer>

<script>
  function toggleLanguage() {
    const esElements = document.querySelectorAll('.lang-es');
    const enElements = document.querySelectorAll('.lang-en');
    const isSpanish = document.documentElement.lang === 'es';
    
    esElements.forEach(el => el.style.display = isSpanish ? 'none' : 'block');
    enElements.forEach(el => el.style.display = isSpanish ? 'block' : 'none');
    document.documentElement.lang = isSpanish ? 'en' : 'es';
    document.getElementById("language-toggle").innerText = isSpanish ? "Español" : "English";
  }

  // Ocultar inglés al cargar
  window.onload = () => {
    document.querySelectorAll('.lang-en').forEach(el => el.style.display = 'none');
  }
</script>

</body>
</html>
