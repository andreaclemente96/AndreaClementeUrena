<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Andrea Clemente-Ureña - Portfolio</title>
  <style>
    body {
      font-family: "Segoe UI", sans-serif;
      margin: 0;
      padding: 2rem;
      line-height: 1.7; /* Más espacio entre líneas */
      background-color: #f7f9fc;
      color: #333;
      font-size: 1.2rem; /* Texto más grande */
    }
    p, li, td {
      text-align: justify;
      text-justify: inter-word;
      font-size: 1.2rem; /* Texto más grande */
    }
    header h1 {
      text-align: center;
      color: #2c3e50;
      font-size: 2.5rem; /* Título principal más grande */
      margin-bottom: 1rem;
    }
    header p {
      text-align: center;
      color: #2c3e50;
      font-size: 1.4rem;
      margin-bottom: 1.5rem;
    }
    img {
      border-radius: 10px;
      margin: 1rem auto;
      display: block;
      max-width: 100%;
    }
    /* Imagen de bienvenida grande */
    #bienvenida img.section-img {
      width: 900px;
      max-width: 90%;
      margin: 2rem auto;
    }
    .section-title {
      text-align: center;
      margin: 3rem 0 1.5rem;
      color: #2c3e50;
      font-size: 2rem; /* Títulos de sección más grandes */
      font-weight: bold;
    }
    /* Estilo para secciones que se muestran directamente */
    .direct-section {
      background-color: white;
      padding: 2rem;
      border-radius: 10px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
      margin: 2rem 0;
    }
    /* Proyectos - imágenes grandes con título */
    .project-container {
      margin: 3rem 0;
    }
    .project-title {
      text-align: center;
      font-size: 1.8rem;
      font-weight: bold;
      color: #2c3e50;
      margin-bottom: 1.5rem;
    }
    .project-image {
      width: 900px;
      max-width: 95%;
      margin: 0 auto 2rem;
    }
    .project-image img {
      width: 100%;
      box-shadow: 0 4px 15px rgba(0,0,0,0.1);
    }
    .project-description {
      max-width: 900px;
      margin: 0 auto;
      font-size: 1.2rem;
    }
    /* Botón de idioma */
    #language-toggle {
      position: fixed;
      top: 15px;
      right: 15px;
      padding: 10px 15px;
      background: #2c3e50;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      z-index: 1000;
      font-size: 1.1rem;
    }
    /* Formulario de contacto */
    form {
      margin: 3rem auto;
      background-color: white;
      padding: 2rem;
      border-radius: 10px;
      max-width: 700px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    }
    form h2 {
      text-align: center;
      font-size: 1.8rem;
      margin-bottom: 1.5rem;
    }
    form label {
      display: block;
      margin-top: 1.5rem;
      font-size: 1.2rem;
    }
    form input, form textarea {
      width: 100%;
      padding: 12px;
      margin-top: 8px;
      border: 1px solid #ddd;
      border-radius: 6px;
      font-size: 1.1rem;
    }
    form input[type="submit"] {
      background-color: #2c3e50;
      color: white;
      cursor: pointer;
      border: none;
      padding: 14px 24px;
      font-size: 1.2rem;
      margin-top: 1.5rem;
      transition: background-color 0.3s;
    }
    form input[type="submit"]:hover {
      background-color: #1a252f;
    }
    /* Listas */
    ul {
      padding-left: 2rem;
    }
    li {
      margin-bottom: 1.2rem;
      font-size: 1.2rem;
    }
    /* Tablas */
    table {
      width: 100%;
      border-collapse: collapse;
      margin: 1.5rem 0;
    }
    td {
      padding: 12px 15px;
      border-bottom: 1px solid #eee;
      vertical-align: top;
    }
    td:first-child {
      font-weight: bold;
      width: 30%;
    }
    /* Footer */
    footer {
      text-align: center;
      font-style: italic;
      margin: 4rem 0 2rem;
      font-size: 1.3rem;
      color: #2c3e50;
      padding: 1.5rem;
      background-color: white;
      border-radius: 10px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    }
    /* Ocultar elementos inglés inicialmente */
    .lang-en { display: none; }
  </style>
</head>
<body>

<button id="language-toggle" onclick="toggleLanguage()">English</button>

<header>
  <h1>
    <span class="lang-es">👩‍🔬 Andrea Clemente-Ureña</span>
    <span class="lang-en">👩‍🔬 Andrea Clemente-Ureña</span>
  </h1>
  <p>
    <span class="lang-es">Aquí comparto mi trayectoria en <strong>biología</strong>, <strong>bioinformática</strong>, <strong>robótica</strong> y <strong>visión computacional 3D</strong>.</span>
    <span class="lang-en">Here I share my journey in <strong>biology</strong>, <strong>bioinformatics</strong>, <strong>robotics</strong> and <strong>3D computer vision</strong>.</span>
  </p>
  <p>
    <span class="lang-es"><strong>Investigadora predoctoral</strong> en UPM y CRF-INIA-CSIC | Proyecto: Transformación digital de la conservación y mejora vegetal</span>
    <span class="lang-en"><strong>Predoctoral Researcher</strong> at UPM and CRF-INIA-CSIC | Project: Digital Transformation of Plant Conservation and Improvement</span>
  </p>
</header>

<!-- Sección: Bienvenida -->
<section id="bienvenida" class="direct-section">
  <h2 class="section-title">
    <span class="lang-es">¡Bienvenid@ a mi portfolio!</span>
    <span class="lang-en">Welcome to my portfolio!</span>
  </h2>
  <img class="section-img" src="beautiful-landscape-with-rainbow-plants.jpg" alt="Bienvenida">
  <p>
    <span class="lang-es">Este espacio reúne mi trayectoria en <strong>biología</strong>, <strong>bioinformática</strong>, <strong>robótica</strong> y <strong>visión computacional 3D</strong>. Actualmente desarrollo herramientas avanzadas para el <strong>fenotipado de cultivos</strong> y la <strong>caracterización de estructuras vegetales</strong>, aplicando aprendizaje automático y análisis de datos.</span>
    <span class="lang-en">This space brings together my journey in <strong>biology</strong>, <strong>bioinformatics</strong>, <strong>robotics</strong> and <strong>3D computer vision</strong>. I currently develop advanced tools for <strong>crop phenotyping</strong> and <strong>plant structure characterization</strong> using machine learning and data analysis.</span>
  </p>
  <p>
    <span class="lang-es">📍 Investigadora predoctoral en la Universidad Politécnica de Madrid (UPM) y el Centro de Recursos Fitogenéticos (CRF-INIA-CSIC), dentro del proyecto <strong>Transformación digital de las actividades de conservación y mejora vegetal</strong>.</span>
    <span class="lang-en">📍 Predoctoral researcher at the Polytechnic University of Madrid (UPM) and the Plant Genetic Resources Center (CRF-INIA-CSIC), within the project <strong>Digital Transformation of Plant Conservation and Improvement</strong>.</span>
  </p>
</section>

<!-- Sección: Mi primer contacto con la investigación -->
<section id="primer-contacto-section" class="direct-section">
  <h2 class="section-title">
    <span class="lang-es">💡 Mi primer contacto con la investigación</span>
    <span class="lang-en">💡 My first encounter with research</span>
  </h2>
  <p>
    <span class="lang-es">Mi primer contacto con la investigación fue en 1º de Bachillerato, cuando desarrollé un proyecto sobre la <em>síntesis de bioplásticos a partir de la leche de vaca</em> en las asignaturas de Biología y Técnicas Experimentales en Ciencias. Ese mismo año participé en el <strong>Finde Científico</strong>, formando parte de un equipo que realizaba experimentos de química visual para la divulgación científica.</span>
    <span class="lang-en">My first encounter with research was in the first year of high school when I developed a project on the <em>synthesis of bioplastics from cow's milk</em> in Biology and Experimental Techniques classes. That same year, I participated in the Science Weekend (Finde Científico), as part of a team performing visual chemistry experiments for science outreach.</span>
  </p>
  
  <div class="project-container">
    <div class="project-title">
      <span class="lang-es">Síntesis de bioplásticos</span>
      <span class="lang-en">Bioplastics Synthesis</span>
    </div>
    <div class="project-image">
      <img src="laboratory-samples-arrangement.jpg" alt="Síntesis de bioplásticos">
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
  </div>
</section>

<!-- Sección: Proyectos destacados -->
<section id="proyectos-section" class="direct-section">
  <h2 class="section-title">
    <span class="lang-es">🚀 Proyectos destacados</span>
    <span class="lang-en">🚀 Featured Projects</span>
  </h2>
  
  <!-- Proyecto 1 -->
  <div class="project-container">
    <div class="project-title">
      <span class="lang-es">Fenotipado de alto rendimiento</span>
      <span class="lang-en">High-throughput phenotyping</span>
    </div>
    <div class="project-image">
      <img src="3461225.jpg" alt="Fenotipado de cultivos">
    </div>
    <div class="project-description">
      <p>
        <span class="lang-es">Fenotipado automatizado de cultivos con robótica y visión computacional. Diseño experimental y análisis de datos fenotípicos.</span>
        <span class="lang-en">Automated crop phenotyping with robotics and computer vision. Experimental design and phenotypic data analysis.</span>
      </p>
    </div>
  </div>
  
  <!-- Proyecto 2 -->
  <div class="project-container">
    <div class="project-title">
      <span class="lang-es">Bioinformática y análisis ómico</span>
      <span class="lang-en">Bioinformatics and omic analysis</span>
    </div>
    <div class="project-image">
      <img src="https://github.com/user-attachments/assets/8dfa2628-f892-4078-bde3-3915150bed34" alt="Bioinformática">
    </div>
    <div class="project-description">
      <p>
        <span class="lang-es">TFM: Identificación y caracterización de tRFs sobreexpresados en enfermedad de Huntington. DOI: <a href="https://doi.org/10.13140/RG.2.2.33680.32001" target="_blank">10.13140/RG.2.2.33680.32001</a></span>
        <span class="lang-en">Master's Thesis: Identification and characterization of overexpressed tRFs in Huntington's disease. DOI: <a href="https://doi.org/10.13140/RG.2.2.33680.32001" target="_blank">10.13140/RG.2.2.33680.32001</a></span>
      </p>
    </div>
  </div>
  
  <!-- Proyecto 3 -->
  <div class="project-container">
    <div class="project-title">
      <span class="lang-es">Genética molecular y citología</span>
      <span class="lang-en">Molecular genetics and cytology</span>
    </div>
    <div class="project-image">
      <img src="https://github.com/user-attachments/assets/b740f460-1160-4a35-90c6-b3b2e5861f23" alt="Genética molecular">
    </div>
    <div class="project-description">
      <p>
        <span class="lang-es">
          TFG: Caracterización estructural de genes codificantes de proteínas ribosómicas en Leishmania. DOI: 
          <a href="https://doi.org/10.13140/RG.2.2.10192.21767" target="_blank">10.13140/RG.2.2.10192.21767</a>. 
          Participación mencionada en el 
          <a href="https://www.cbm.uam.es/wp-content/uploads/2024/07/CBM-Scientific-Report-2021-2022.pdf" target="_blank">
            Informe Científico del CBMSO-CSIC 2021–2022
          </a>.
        </span>
        <span class="lang-en">
          Bachelor's Thesis: Structural characterization of genes coding for ribosomal proteins in Leishmania. DOI: 
          <a href="https://doi.org/10.13140/RG.2.2.10192.21767" target="_blank">10.13140/RG.2.2.10192.21767</a>. 
          Participation mentioned in the 
          <a href="https://www.cbm.uam.es/wp-content/uploads/2024/07/CBM-Scientific-Report-2021-2022.pdf" target="_blank">
            CBMSO-CSIC Scientific Report 2021–2022
          </a>.
        </span>
      </p>
    </div>
  </div>
  
  <!-- Proyecto 4 -->
  <div class="project-container">
    <div class="project-title">
      <span class="lang-es">Histología e inmunohistoquímica</span>
      <span class="lang-en">Histology and immunohistochemistry</span>
    </div>
    <div class="project-image">
      <img src="https://github.com/user-attachments/assets/73e74b49-a323-40f3-b055-1f3bfaf9750c" alt="Histología">
    </div>
    <div class="project-description">
      <p>
        <span class="lang-es">Proyecto sobre detección inmunohistoquímica de BRCA en cáncer de mama durante el FPII.</span>
        <span class="lang-en">Project on immunohistochemical detection of BRCA in breast cancer during FPII.</span>
      </p>
    </div>
  </div>
  
  <!-- Proyecto 5 -->
  <div class="project-container">
    <div class="project-title">
      <span class="lang-es">Tecnologías inmersivas</span>
      <span class="lang-en">Immersive technologies</span>
    </div>
    <div class="project-image">
      <img src="3162813.jpg" alt="Tecnologías inmersivas">
    </div>
    <div class="project-description">
      <p>
        <span class="lang-es">Colaboración con el Centro de Automática y Robótica (CAR-CSIC-UPM) para desarrollar soluciones con Microsoft HoloLens2 en aplicaciones agrícolas. (Proyecto en fase inicial)</span>
        <span class="lang-en">Collaboration with the Center for Automation and Robotics (CAR-CSIC-UPM) to develop solutions with Microsoft HoloLens2 in agricultural applications. (Initial project)</span>
      </p>
    </div>
  </div>
</section>

<!-- Sección: Formación académica -->
<section id="formacion-section" class="direct-section">
  <h2 class="section-title">
    <span class="lang-es">🎓 Formación académica</span>
    <span class="lang-en">🎓 Academic Education</span>
  </h2>
  <ul>
    <li>
      <span class="lang-es">📘 <strong>Doctorado en Automática y Robótica</strong> (2024 - actualidad)<br>
        Universidad Politécnica de Madrid – INIA-CSIC</span>
      <span class="lang-en">📘 <strong>PhD in Automation and Robotics</strong> (2024 - Present)<br>
        Polytechnic University of Madrid – INIA-CSIC</span>
    </li>
    <li>
      <span class="lang-es">📊 <strong>Máster en Bioinformática y Bioestadística</strong> (2022 - 2024)<br>
        Universitat Oberta de Catalunya / Universitat de Barcelona</span>
      <span class="lang-en">📊 <strong>Master in Bioinformatics and Biostatistics</strong> (2022 - 2024)<br>
        Open University of Catalonia / University of Barcelona</span>
    </li>
    <li>
      <span class="lang-es">🧬 <strong>Grado en Biología</strong> (2016 - 2021)<br>
        Universidad Autónoma de Madrid</span>
      <span class="lang-en">🧬 <strong>Bachelor in Biology</strong> (2016 - 2021)<br>
        Autonomous University of Madrid</span>
    </li>
    <li>
      <span class="lang-es">🔬 <strong>Técnico Superior en Anatomía Patológica y Citología</strong> (2014 - 2016)<br>
        CESUR II</span>
      <span class="lang-en">🔬 <strong>Higher Technician in Pathological Anatomy and Cytology</strong> (2014 - 2016)<br>
        CESUR II</span>
    </li>
  </ul>
</section>

<!-- Sección: Tecnologías y herramientas -->
<section id="tecnologias-section" class="direct-section">
  <h2 class="section-title">
    <span class="lang-es">🛠️ Tecnologías y herramientas</span>
    <span class="lang-en">🛠️ Technologies and Tools</span>
  </h2>
  <table>
    <tr>
      <td><strong><span class="lang-es">Lenguajes</span><span class="lang-en">Languages</span></strong></td>
      <td>Python • R • SQL • BASH • HTML/CSS</td>
    </tr>
    <tr>
      <td><strong><span class="lang-es">Ciencia &amp; Bioinfo</span><span class="lang-en">Science &amp; Bioinformatics</span></strong></td>
      <td>Bioconductor • SPSS • Galaxy • Novopath • Inferencia estadística</td>
    </tr>
    <tr>
      <td><strong><span class="lang-es">IA / Visión</span><span class="lang-en">AI / Vision</span></strong></td>
      <td>OpenCV • PyTorch • TensorFlow • Scikit-learn • Visión 3D</td>
    </tr>
    <tr>
      <td><strong><span class="lang-es">Robótica</span><span class="lang-en">Robotics</span></strong></td>
      <td>Sensores RGB • Sensores Multiespectrales • Sensores LiDAR/ToF • HoloLens 2</td>
    </tr>
    <tr>
      <td><strong><span class="lang-es">Entornos</span><span class="lang-en">Environments</span></strong></td>
      <td>Linux • VS Code • Git • Office</td>
    </tr>
  </table>
</section>

<!-- Sección: Experiencia profesional -->
<section id="experiencia-section" class="direct-section">
  <h2 class="section-title">
    <span class="lang-es">📚 Experiencia profesional</span>
    <span class="lang-en">📚 Professional Experience</span>
  </h2>
  <ul>
    <li>
      <span class="lang-es">🔬 <strong>Investigadora Predoctoral</strong> | INIA-CSIC (2024 - actualidad)<br>
        Fenotipado automatizado de cultivos con robótica y visión computacional. Diseño experimental y análisis de datos fenotípicos.</span>
      <span class="lang-en">🔬 <strong>Predoctoral Researcher</strong> | INIA-CSIC (2024 - Present)<br>
        Automated crop phenotyping with robotics and computer vision. Experimental design and phenotypic data analysis.</span>
    </li>
    <li>
      <span class="lang-es">🧫 <strong>Técnico de Anatomía Patológica</strong> | HM Hospitales (2016)<br>
        Procesamiento y análisis de muestras biológicas y técnicas histológicas.</span>
      <span class="lang-en">🧫 <strong>Pathological Anatomy Technician</strong> | HM Hospitales (2016)<br>
        Processing and analysis of biological samples and histological techniques.</span>
    </li>
    <li>
      <span class="lang-es">📞 <strong>Teleoperadora Comercial</strong> | My Assessor Total (2021)<br>
        Primer contacto con el mundo laboral. Aprender cómo funciona el empleo fuera del ámbito científico.</span>
      <span class="lang-en">📞 <strong>Commercial Operator</strong> | My Assessor Total (2021)<br>
        First contact with the working world. Learning how employment works outside the scientific field.</span>
    </li>
  </ul>
</section>

<!-- Sección: Idiomas -->
<section id="idiomas-section" class="direct-section">
  <h2 class="section-title">
    <span class="lang-es">🌐 Idiomas</span>
    <span class="lang-en">🌐 Languages</span>
  </h2>
  <ul>
    <li><span class="lang-es">🇪🇸 Español: Nativo</span><span class="lang-en">🇪🇸 Spanish: Native</span></li>
    <li><span class="lang-es">🇬🇧 Inglés: Nivel C (APTIS - British Council)</span><span class="lang-en">🇬🇧 English: Level C (APTIS - British Council)</span></li>
    <li><span class="lang-es">🇫🇷 Francés: Nivel A2 (DELF)</span><span class="lang-en">🇫🇷 French: Level A2 (DELF)</span></li>
  </ul>
</section>

<!-- Sección: Contacto -->
<section id="contacto-section" class="direct-section">
  <h2 class="section-title">
    <span class="lang-es">📫 Contacto</span>
    <span class="lang-en">📫 Contact</span>
  </h2>
  <ul>
    <li><span class="lang-es">✉️ Email:</span><span class="lang-en">✉️ Email:</span> <a href="mailto:andeande.ac@gmail.com">andeande.ac@gmail.com</a></li>
    <li><span class="lang-es">🔗 LinkedIn:</span><span class="lang-en">🔗 LinkedIn:</span> <a href="https://www.linkedin.com/in/andreaclementeure%C3%B1a/" target="_blank">linkedin.com/in/andreaclementeureña</a></li>
    <li><span class="lang-es">💻 GitHub:</span><span class="lang-en">💻 GitHub:</span> <a href="https://github.com/andyacment" target="_blank">github.com/andyacment</a></li>
  </ul>
</section>

<!-- Formulario de contacto -->
<form id="contact-form">
  <h2>
    <span class="lang-es">Formulario de Contacto</span>
    <span class="lang-en">Contact Form</span>
  </h2>
  <label for="name">
    <span class="lang-es">Nombre</span>
    <span class="lang-en">Name</span>
  </label>
  <input type="text" id="name" name="name" required>
  
  <label for="email">
    <span class="lang-es">Correo electrónico</span>
    <span class="lang-en">Email</span>
  </label>
  <input type="email" id="email" name="email" required>
  
  <label for="message">
    <span class="lang-es">Mensaje</span>
    <span class="lang-en">Message</span>
  </label>
  <textarea id="message" name="message" rows="6" required></textarea>
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
    if (document.documentElement.lang === 'es') {
      esElements.forEach(el => el.style.display = 'none');
      enElements.forEach(el => el.style.display = 'inline');
      document.documentElement.lang = 'en';
      document.getElementById("language-toggle").innerText = "Español";
    } else {
      enElements.forEach(el => el.style.display = 'none');
      esElements.forEach(el => el.style.display = 'inline');
      document.documentElement.lang = 'es';
      document.getElementById("language-toggle").innerText = "English";
    }
  }

  document.getElementById("contact-form").addEventListener("submit", function(e) {
    e.preventDefault();
    alert(
      document.documentElement.lang === 'es' 
        ? "Formulario enviado. Gracias por tu mensaje." 
        : "Form submitted. Thank you for your message."
    );
    this.reset();
  });
</script>

</body>
</html>
