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
      line-height: 1.6;
      background-color: #f7f9fc;
      color: #333;
      font-size: 1.1rem; /* Texto más grande */
    }
    p, li, td {
      text-align: justify; /* Texto justificado */
      text-justify: inter-word;
    }
    header h1 {
      text-align: center;
      color: #2c3e50;
      font-size: 2.2rem; /* Título principal más grande */
    }
    header p {
      text-align: center;
      color: #2c3e50;
      font-size: 1.2rem;
    }
    /* Todas las imágenes se centran y se ajustan */
    img {
      border-radius: 10px;
      margin: 1rem auto;
      cursor: pointer;
      display: block;
      max-width: 100%;
    }
    /* Imagen de bienvenida 3 veces más grande */
    #bienvenida img.section-img {
      width: 900px;
      max-width: 90%;
    }
    /* Imagenes principales de sección: tamaño aproximado */
    .section-img {
      width: 300px;
    }
    .section-title {
      text-align: center;
      margin: 1.5rem 0 0.5rem;
      color: #2c3e50;
      font-size: 1.8rem; /* Títulos de sección más grandes */
    }
    .content {
      display: none;
      margin-top: 10px;
    }
    /* Estilo para los títulos de las imágenes de proyectos */
    .project-image-title {
      text-align: center;
      font-weight: bold;
      margin: 1rem 0 0.5rem;
      font-size: 1.3rem;
      color: #2c3e50;
    }
    /* Imágenes de proyectos más grandes */
    .project-content img {
      width: 900px;
      max-width: 90%;
    }
    /* Contenedor de imágenes de proyecto */
    .project-images-container {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 2rem;
      margin: 2rem 0;
    }
    /* Botón de idioma */
    #language-toggle {
      position: fixed;
      top: 10px;
      right: 10px;
      padding: 8px 12px;
      background: #2c3e50;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      z-index: 1000;
      font-size: 1rem;
    }
    /* Formulario de contacto */
    form {
      margin-top: 2rem;
      background-color: #eef4fa;
      padding: 1.5rem;
      border-radius: 10px;
      max-width: 600px;
      margin-left: auto;
      margin-right: auto;
    }
    form label {
      display: block;
      margin-top: 1rem;
      font-size: 1.1rem;
    }
    form input, form textarea {
      width: 100%;
      padding: 10px;
      margin-top: 8px;
      margin-bottom: 16px;
      border: 1px solid #ccc;
      border-radius: 4px;
      font-size: 1rem;
    }
    form input[type="submit"] {
      background-color: #2c3e50;
      color: white;
      cursor: pointer;
      border: none;
      padding: 12px 20px;
      font-size: 1.1rem;
    }
    /* Traducción: inicialmente mostramos el español y ocultamos el inglés */
    .lang-en { display: none; }
    /* Estilos para las miniaturas de los proyectos */
    .project-thumbnails {
      display: flex;
      gap: 15px;
      flex-wrap: wrap;
      justify-content: center;
      margin: 20px 0;
    }
    .thumbnail {
      width: 120px; /* Tamaño un poco más grande */
      border: 1px solid #ccc;
      border-radius: 5px;
      overflow: hidden;
      transition: transform 0.3s;
    }
    .thumbnail:hover {
      transform: scale(1.05);
    }
    .thumbnail img {
      width: 100%;
      display: block;
    }
    /* Footer en cursiva y centrado */
    footer {
      text-align: center;
      font-style: italic;
      margin-top: 3rem;
      font-size: 1.2rem;
      padding: 1rem;
      color: #2c3e50;
    }
    /* Mejoras para listas */
    ul {
      padding-left: 1.5rem;
    }
    li {
      margin-bottom: 0.8rem;
    }
  </style>
</head>
<body>

<!-- Botón para alternar idioma -->
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

<!-- Sección: Bienvenida (siempre visible) -->
<section id="bienvenida">
  <h2 class="section-title">
    <span class="lang-es">¡Bienvenid@ a mi portfolio!</span>
    <span class="lang-en">Welcome to my portfolio!</span>
  </h2>
  <img class="section-img" src="beautiful-landscape-with-rainbow-plants.jpg" alt="Bienvenida">
  <div class="content" style="display: block;"> 
    <p>
      <span class="lang-es">Este espacio reúne mi trayectoria en <strong>biología</strong>, <strong>bioinformática</strong>, <strong>robótica</strong> y <strong>visión computacional 3D</strong>. Actualmente desarrollo herramientas avanzadas para el <strong>fenotipado de cultivos</strong> y la <strong>caracterización de estructuras vegetales</strong>, aplicando aprendizaje automático y análisis de datos. <strong>Si te interesa mi trabajo, ¡Haz click en las siguientes imágenes!</strong> </span>
      <span class="lang-en">This space brings together my journey in <strong>biology</strong>, <strong>bioinformatics</strong>, <strong>robotics</strong> and <strong>3D computer vision</strong>. I currently develop advanced tools for <strong>crop phenotyping</strong> and <strong>plant structure characterization</strong> using machine learning and data analysis. <strong>If you're interested in my work, click on the following images!</strong></span>
    </p>
    <p>
      <span class="lang-es">📍 Investigadora predoctoral en la Universidad Politécnica de Madrid (UPM) y el Centro de Recursos Fitogenéticos (CRF-INIA-CSIC), dentro del proyecto <strong>Transformación digital de las actividades de conservación y mejora vegetal</strong>.</span>
      <span class="lang-en">📍 Predoctoral researcher at the Polytechnic University of Madrid (UPM) and the Plant Genetic Resources Center (CRF-INIA-CSIC), within the project <strong>Digital Transformation of Plant Conservation and Improvement</strong>.</span>
    </p>
  </div>
</section>

<!-- Sección: Mi primer contacto con la investigación -->
<section id="primer-contacto-section">
  <h2 class="section-title">
    <span class="lang-es">💡 Mi primer contacto con la investigación</span>
    <span class="lang-en">💡 My first encounter with research</span>
  </h2>
  <img class="section-img" src="composed-pencils-chalkboard.jpg" alt="Mi primer contacto con la investigación" onclick="toggleContent('primer_contacto')">
  <div id="primer_contacto" class="content">
    <p>
      <span class="lang-es">Mi primer contacto con la investigación fue en 1º de Bachillerato, cuando desarrollé un proyecto sobre la <em>síntesis de bioplásticos a partir de la leche de vaca</em> en las asignaturas de Biología y Técnicas Experimentales en Ciencias. Ese mismo año participé en el <strong>Finde Científico</strong>, formando parte de un equipo que realizaba experimentos de química visual para la divulgación científica.</span>
      <span class="lang-en">My first encounter with research was in the first year of high school when I developed a project on the <em>synthesis of bioplastics from cow's milk</em> in Biology and Experimental Techniques classes. That same year, I participated in the Science Weekend (Finde Científico), as part of a team performing visual chemistry experiments for science outreach.</span>
    </p>
    <div class="project-images-container">
      <div>
        <div class="project-image-title">
          <span class="lang-es">Síntesis de bioplásticos</span>
          <span class="lang-en">Bioplastics Synthesis</span>
        </div>
        <img src="laboratory-samples-arrangement.jpg" alt="Síntesis de bioplásticos">
      </div>
      <div>
        <div class="project-image-title">
          <span class="lang-es">Finde Científico</span>
          <span class="lang-en">Science Weekend</span>
        </div>
        <img src="lab-glassware-with-colored-liquids-assortment.jpg" alt="Finde Científico">
      </div>
    </div>
  </div>
</section>

<!-- Sección: Proyectos destacados -->
<section id="proyectos-section">
  <h2 class="section-title">
    <span class="lang-es">🚀 Proyectos destacados</span>
    <span class="lang-en">🚀 Featured Projects</span>
  </h2>
  <img class="section-img" src="https://via.placeholder.com/300?text=Proyectos" alt="Proyectos Destacados" onclick="toggleContent('proyectos-thumbnails')">
  <div id="proyectos-thumbnails" class="content">
    <!-- Miniaturas de cada proyecto -->
    <div class="project-thumbnails">
      <div class="thumbnail" title="Fenotipado de alto rendimiento" onclick="toggleContent('proyecto1')">
        <img src="3461225.jpg" alt="Miniatura 1">
      </div>
      <div class="thumbnail" title="Bioinformática y análisis ómico" onclick="toggleContent('proyecto2')">
        <img src="https://github.com/user-attachments/assets/8dfa2628-f892-4078-bde3-3915150bed34" alt="Miniatura 2">
      </div>
      <div class="thumbnail" title="Genética molecular y citología" onclick="toggleContent('proyecto3')">
        <img src="https://github.com/user-attachments/assets/b740f460-1160-4a35-90c6-b3b2e5861f23" alt="Miniatura 3">
      </div>
      <div class="thumbnail" title="Histología e inmunohistoquímica" onclick="toggleContent('proyecto4')">
        <img src="https://github.com/user-attachments/assets/73e74b49-a323-40f3-b055-1f3bfaf9750c" alt="Miniatura 4">
      </div>
      <div class="thumbnail" title="Exploración con tecnologías inmersivas" onclick="toggleContent('proyecto5')">
        <img src="3162813.jpg" alt="Miniatura 5">
      </div>
    </div>
    
    <!-- Detalles de cada proyecto -->
    <div id="proyecto1" class="content project-content">
      <h3 class="project-image-title">
        <span class="lang-es">Fenotipado de alto rendimiento</span>
        <span class="lang-en">High-throughput phenotyping</span>
      </h3>
      <p>
        <span class="lang-es">Fenotipado automatizado de cultivos con robótica y visión computacional. Diseño experimental y análisis de datos fenotípicos.</span>
        <span class="lang-en">Automated crop phenotyping with robotics and computer vision. Experimental design and phenotypic data analysis.</span>
      </p>
      <div class="project-images-container">
        <img src="3461225.jpg" alt="Fenotipado de cultivos">
      </div>
    </div>
    
    <div id="proyecto2" class="content project-content">
      <h3 class="project-image-title">
        <span class="lang-es">Bioinformática y análisis ómico</span>
        <span class="lang-en">Bioinformatics and omic analysis</span>
      </h3>
      <p>
        <span class="lang-es">TFM: Identificación y caracterización de tRFs sobreexpresados en enfermedad de Huntington. DOI: <a href="https://doi.org/10.13140/RG.2.2.33680.32001" target="_blank">10.13140/RG.2.2.33680.32001</a></span>
        <span class="lang-en">Master's Thesis: Identification and characterization of overexpressed tRFs in Huntington's disease. DOI: <a href="https://doi.org/10.13140/RG.2.2.33680.32001" target="_blank">10.13140/RG.2.2.33680.32001</a></span>
      </p>
      <div class="project-images-container">
        <img src="https://github.com/user-attachments/assets/8dfa2628-f892-4078-bde3-3915150bed34" alt="Bioinformática">
      </div>
    </div>
    
    <div id="proyecto3" class="content project-content">
      <h3 class="project-image-title">
        <span class="lang-es">Genética molecular y citología</span>
        <span class="lang-en">Molecular genetics and cytology</span>
      </h3>
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
      <div class="project-images-container">
        <img src="https://github.com/user-attachments/assets/b740f460-1160-4a35-90c6-b3b2e5861f23" alt="Genética molecular">
      </div>
    </div>
    
    <div id="proyecto4" class="content project-content">
      <h3 class="project-image-title">
        <span class="lang-es">Histología e inmunohistoquímica</span>
        <span class="lang-en">Histology and immunohistochemistry</span>
      </h3>
      <p>
        <span class="lang-es">Proyecto sobre detección inmunohistoquímica de BRCA en cáncer de mama durante el FPII.</span>
        <span class="lang-en">Project on immunohistochemical detection of BRCA in breast cancer during FPII.</span>
      </p>
      <div class="project-images-container">
        <img src="https://github.com/user-attachments/assets/73e74b49-a323-40f3-b055-1f3bfaf9750c" alt="Histología">
      </div>
    </div>
    
    <div id="proyecto5" class="content project-content">
      <h3 class="project-image-title">
        <span class="lang-es">Tecnologías inmersivas</span>
        <span class="lang-en">Immersive technologies</span>
      </h3>
      <p>
        <span class="lang-es">Colaboración con el Centro de Automática y Robótica (CAR-CSIC-UPM) para desarrollar soluciones con Microsoft HoloLens2 en aplicaciones agrícolas. (Proyecto en fase inicial)</span>
        <span class="lang-en">Collaboration with the Center for Automation and Robotics (CAR-CSIC-UPM) to develop solutions with Microsoft HoloLens2 in agricultural applications. (Initial project)</span>
      </p>
      <div class="project-images-container">
        <img src="3162813.jpg" alt="Tecnologías inmersivas">
      </div>
    </div>
  </div>
</section>

<!-- Resto de las secciones (Formación, Tecnologías, Experiencia, Idiomas, Contacto) -->
<!-- Se mantienen igual que en el código anterior, solo cambia el estilo general -->

<footer>
  <p>
    <span class="lang-es">"La IA no es el enemigo, es la lupa que amplifica lo que la ciencia aún no alcanza." 🤖🔬🌍</span>
    <span class="lang-en">"AI is not the enemy; it is the magnifying glass that amplifies what science has not yet reached." 🤖🔬🌍</span>
  </p>
</footer>

<script>
  function toggleContent(id) {
    var content = document.getElementById(id);
    content.style.display = (content.style.display === "block") ? "none" : "block";
  }

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
