<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Andrea Clemente-Ureña - Portfolio</title>
  <style>
    :root {
      --primary-color: #2e7d32;  /* Verde principal */
      --secondary-color: #388e3c;  /* Verde secundario */
      --accent-color: #a5d6a7;  /* Verde claro */
      --background: #f0f4f3;  /* Fondo verde claro */
    }
    body {
      font-family: "Segoe UI", sans-serif;
      margin: 0;
      padding: 2rem;
      line-height: 1.7;
      background-color: var(--background);
      color: #2d3436;
      font-size: 1.2rem;
    }
    p, li, td {
      text-align: justify;
      text-justify: inter-word;
      font-size: 1.2rem; /* Texto más grande */
    }
    header h1 {
      text-align: center;
      color: var(--primary-color);
      font-size: 2.5rem; /* Título principal más grande */
      margin-bottom: 1rem;
    }
    header p {
      text-align: center;
      color: var(--primary-color);
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
      color: var(--primary-color);
      font-size: 2rem; /* Títulos de sección más grandes */
      font-weight: bold;
    }
    /* Estilo para secciones que se muestran directamente */
    .direct-section {
      background: linear-gradient(145deg, #ffffff 0%, #f0f4f3 100%);
      border: 1px solid var(--accent-color);
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
      color: var(--secondary-color);
      margin-bottom: 1.5rem;
    }
    .project-image {
      width: 900px;
      max-width: 95%;
      margin: 0 auto 2rem;
    }
    .project-image img:not(.section-img) {
      width: 300px;
      max-width: 100%;
      height: auto;
      cursor: pointer;
      transition: transform 0.3s;
    }
    .project-image img:hover:not(.section-img) {
      transform: scale(1.05);
    }
    .project-description {
      display: none;
      padding: 1rem;
      background-color: rgba(165, 214, 167, 0.2);
      border-radius: 10px;
      margin-top: 1rem;
    }
    .project-description.active {
      display: block;
      animation: fadeIn 0.3s ease-in;
    }
    .centered-link {
      text-align: center;
      display: block;
    }
    /* Botón de idioma */
    #language-toggle {
      position: fixed;
      top: 15px;
      right: 15px;
      padding: 10px 15px;
      background: var(--secondary-color);
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      z-index: 1000;
      font-size: 1.1rem;
    }
    #image-credits {
      font-size: 0.8rem; 
      text-align: right; /* Alineación a la derecha */
      margin-top: 10px; 
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
      background-color: var(--secondary-color);
      color: white;
      cursor: pointer;
      border: none;
      padding: 14px 24px;
      font-size: 1.2rem;
      margin-top: 1.5rem;
      transition: background-color 0.3s;
    }
    form input[type="submit"]:hover {
      background-color: #1b5e20;
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
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    /* Fix para toggle de idioma */
    .lang-en { display: none !important; }
    [lang="en"] .lang-en { display: inline !important; }
    [lang="en"] .lang-es { display: none !important; }

    /* Tabla de navegación */
    .nav-table {
      width: 100%;
      margin: 2rem 0;
      border-collapse: collapse;
    }
    .nav-table td {
      padding: 1rem;
      text-align: center;
      border: 2px solid var(--accent-color);
      transition: all 0.3s;
    }
    .nav-table td:hover {
      background-color: var(--accent-color);
      cursor: pointer;
      transform: scale(1.05);
    }
    .nav-table a {
      text-decoration: none;
      color: var(--primary-color);
      font-weight: bold;
      display: block;
    }
    .centrado {
      text-align: center;
    }
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
    <span class="lang-es">Aquí comparto mi trayectoria en <strong>biología</strong>, <strong>bioinformática</strong> y en el desarrollo de sistemas de <strong>fenotipado de alto rendimiento</strong> mediante <strong>robótica</strong> e <strong>inteligencia artificial</strong>, con énfasis en <strong>visión computacional 3D</strong>.</span>
    <span class="lang-en">I share my background in <strong>biology</strong>, <strong>bioinformatics</strong>, and the development of <strong>high-throughput phenotyping</strong> systems using <strong>robotics</strong> and <strong>artificial intelligence</strong>, with a focus on <strong>3D computer vision</strong>.</span>
  </p>
<div class="lang-es">
  <p><strong>Investigadora predoctoral</strong> en la <strong>Universidad Politécnica de Madrid (UPM)</strong> y el <strong>Centro de Recursos Fitogenéticos (CRF)</strong> del 
  <strong>Instituto Nacional de Investigación y Tecnología Agraria y Alimentaria (INIA)</strong>, parte del <strong>Consejo Superior de Investigaciones Científicas (CSIC)</strong>.</p>
  <p>Proyecto: Transformación digital de las actividades de conservación y mejora vegetal mediante fenotipado de alto rendimiento (HTP).</p>
</div>

<div class="lang-en">
  <p><strong>PhD researcher</strong> at the <strong>Technical University of Madrid (UPM)</strong> and the 
  <strong>Center for Plant Genetic Resources (CRF)</strong> at the <strong>National Institute for Agricultural and Food Research and Technology (INIA)</strong>, which is part of the <strong>Spanish National Research Council (CSIC)</strong>.</p>
  <p>Project: Digital transformation of plant genetic resource conservation and crop improvement activities through high-throughput phenotyping (HTP).</p>
</div>

</header>

<section id="bienvenida" class="direct-section">
  <h2 class="section-title">
    <span class="lang-es">¡Bienvenid@ a mi portfolio!</span>
    <span class="lang-en">Welcome to my portfolio!</span>
  </h2>
  
  <img class="section-img" src="beautiful-landscape-with-rainbow-plants.jpg" alt="Bienvenida">
  
<!-- Español -->
<div class="lang-es">
  <p>Actualmente desarrollo herramientas avanzadas para el <strong>fenotipado de alto rendimiento (HTP)</strong> aplicado a <strong>cultivos</strong> y a la <strong>caracterización estructural de plantas</strong>, utilizando <strong>Deep Learning</strong> y <strong>análisis computacional de rasgos fenotípicos</strong>.</p>
  <p class="centrado"><strong>¡Haz clic en las imágenes para ver mis proyectos!</strong></p>
</div>

<!-- Inglés -->
<div class="lang-en">
  <p>I currently develop advanced tools for <strong>high-throughput phenotyping (HTP)</strong> applied to <strong>crop analysis</strong> and <strong>plant structural characterization</strong>, using <strong>Deep Learning</strong> and <strong>computational analysis of phenotypic traits</strong>.</p>
  <p class="centrado"><strong>Click on the images to explore my projects!</strong></p>
</div>

<p class="centered-link">
    <a href="#autorreflexion-section" class="lang-es">🧠 Leer sobre mi autorreflexión</a>  
    <a href="#autorreflexion-section" class="lang-en">🧠 Read about my self-reflection</a>
  </p>
</section>

<section class="direct-section">
  <table class="nav-table">
    <tr>
      <td>
        <a href="#primer-contacto-section">
          <span class="lang-es">Mi primer contacto con la investigación</span>
          <span class="lang-en">My initial experience with research</span>
        </a>
      </td>
      <td>
        <a href="#proyectos-section">
          <span class="lang-es">Proyectos destacados</span>
          <span class="lang-en">Featured Projects</span>
        </a>
      </td>
      <td>
        <a href="#formacion-section">
          <span class="lang-es">Formación académica</span>
          <span class="lang-en">Academic Education</span>
        </a>
      </td>
      <td>
        <a href="#tecnologias-section">
          <span class="lang-es">Tecnologías y herramientas</span>
          <span class="lang-en">Technologies &amp; Tools</span>
        </a>
      </td>
      <td>
        <a href="#experiencia-section">
          <span class="lang-es">Experiencia Profesional</span>
          <span class="lang-en">Professional Experience</span>
        </a>
      </td>
      <td>
        <a href="#idiomas-section">
          <span class="lang-es">Idiomas</span>
          <span class="lang-en">Languages</span>
        </a>
      </td>
      <td>
        <a href="#contacto-section">
          <span class="lang-es">Contacto</span>
          <span class="lang-en">Contact</span>
        </a>
      </td>
    </tr>
  </table>
</section>

<!-- Sección: Mi primer contacto con la investigación -->
<section id="primer-contacto-section" class="direct-section">
  <h2 class="section-title">
    <span class="lang-es">💡 Mi primer contacto con la investigación</span>
    <span class="lang-en">💡 My first encounter with research</span>
  </h2>

  <p>
    <span class="lang-es">
      Mi primer contacto con la investigación fue en 1º de Bachillerato en el <strong>IES Alameda de Osuna</strong>, donde desarrollé un proyecto sobre la <em>síntesis de bioplásticos a partir de leche de vaca</em> en las asignaturas de Biología y Técnicas Experimentales en Ciencias. Ese mismo año participé en el <strong>Finde Científico</strong> con el proyecto <em>“De la magia del arco iris al modelo de Bohr”</em>, formando parte de un equipo dedicado a la divulgación científica mediante experimentos de química visual.  
      <br>El Finde Científico es una feria organizada por la <strong>Fundación Española para la Ciencia y la Tecnología (FECYT)</strong> y el <strong>Museo Nacional de Ciencia y Tecnología (MUNCYT)</strong>, con la colaboración de <strong>Obra Social “la Caixa”</strong>.
    </span>

    <span class="lang-en">
      My first experience with research took place during the first year of upper secondary school at <strong>IES Alameda de Osuna</strong>, where I developed a project on the <em>synthesis of bioplastics from cow’s milk</em> in Biology and Experimental Science Techniques. That same year, I took part in the <strong>Finde Científico</strong> with the project <em>“De la magia del arco iris al modelo de Bohr”</em>, as part of a team focused on science outreach through visual chemistry experiments.  
      <br>The Finde Científico is a science fair organized by the <strong>Spanish Foundation for Science and Technology (FECYT)</strong> and the <strong>National Museum of Science and Technology (MUNCYT)</strong>, with support from <strong>Obra Social “la Caixa”</strong>.
    </span>
  </p>

  <div class="project-container">
    <div class="project-title">
      <span class="lang-es">Ejemplo de imagen de síntesis de bioplásticos</span>
      <span class="lang-en">Example image for bioplastics Synthesis</span>
    </div>
    <div class="project-image">
      <img src="laboratory-samples-arrangement.jpg" alt="Síntesis de bioplásticos">
    </div>
  </div>

  <div class="project-container">
    <div class="project-title">
      <span class="lang-es">Ejemplo de lo que hice en el Finde Científico</span>
      <span class="lang-en">Example of what I did at the &quot;Finde Científico&quot;</span>
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
        <span class="lang-es">
          Mi tesis doctoral se centra en el desarrollo de un sistema de <strong>fenotipado vegetal de alto rendimiento</strong> mediante robótica autónoma, <strong>visión computacional 3D</strong> e <strong>imagen hiperespectral</strong>. Trabajo con <strong>datos obtenidos de cámaras RGB e hiperespectrales</strong> para entrenar modelos de inteligencia artificial que permitan reconstrucciones 3D, segmentación de estructuras vegetales y detección de estrés.
          <br><br>
          Colaboro activamente con el <strong>Centro de Automática y Robótica (CAR, CSIC-UPM)</strong> y la empresa tecnológica <strong>INYCOM</strong> en el marco del contrato predoctoral <strong>MOMENTUM MMT24-PTI AGROFOR</strong>. También participo en el desarrollo del futuro servicio científico-técnico <strong>PTI AGRO4FOOD</strong>.
          <br><br>
          En 2025 participé en la escuela de verano de inteligencia artificial organizada por <strong>AIHUB-CSIC</strong> en Zaragoza, donde presenté el póster titulado <em>“IA y visión 3D hiperespectral para fenotipado de alto rendimiento”</em>.
        </span>

        <span class="lang-en">
          My PhD thesis focuses on developing a <strong>high-throughput plant phenotyping</strong> system using autonomous robotics, <strong>3D computer vision</strong>, and <strong>hyperspectral imaging</strong>. I work with <strong>RGB and hyperspectral data</strong> to train AI models for 3D reconstruction, plant structure segmentation, and stress detection.
          <br><br>
          I actively collaborate with the <strong>Centre for Automation and Robotics (CAR, CSIC-UPM)</strong> and the tech company <strong>INYCOM</strong>, within the framework of the <strong>MOMENTUM MMT24-PTI AGROFOR</strong> predoctoral contract. The project is part of the future <strong>PTI AGRO4FOOD</strong> scientific-technical service.
          <br><br>
          In 2025, I participated in the summer school on artificial intelligence organized by <strong>AIHUB-CSIC</strong> in Zaragoza, where I presented the poster titled <em>“AI and 3D Hyperspectral Vision for High-Throughput Phenotyping”</em>.
        </span>
      </p>

      <!-- Póster interactivo -->
      <div class="poster-section">
        <a href="https://github.com/andreaclemente96/AndreaClementeUrena/blob/andreaclemente96-portfolio/p%C3%B3ster%20hiperespectral.jpg" target="_blank">
          <img src="p%C3%B3ster%20hiperespectral.jpg" alt="Póster IA y visión 3D hiperespectral para fenotipado para alto rendimiento" style="width: 600px; border: 1px solid #ccc;">
        </a>
        <p class="poster-caption">
          <span class="lang-es">Póster: <em>IA y visión 3D hiperespectral para fenotipado de alto rendimiento</em>. Pulsa sobre la imagen para ampliar.</span>
          <span class="lang-en">Poster: <em>AI and 3D Hyperspectral Vision for High-Throughput Phenotyping</em>. Click the image to enlarge.</span>
        </p>
      </div>
    </div>
  </div>
</section>

  
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
        <span class="lang-es">
          He desarrollado una sólida formación en bioinformática y análisis de datos ómicos, combinando herramientas computacionales y métodos estadísticos avanzados. Mi experiencia incluye programación en R y Python, machine learning aplicado a datos biomédicos, análisis multivariante y modelado estadístico.
        </span>
      </p>
      <p>
        <span class="lang-es">
          He trabajado con datos de transcriptómica, genómica y otras fuentes de alto rendimiento, aplicando modelos predictivos e inferencia estadística para extraer información relevante. Además, manejo software especializado para el análisis de datos biomédicos y técnicas de integración de datos ómicos.
          <p>TFM: Identificación y caracterización de tRFs sobreexpresados en enfermedad de Huntington. DOI: 
          <a href="https://doi.org/10.13140/RG.2.2.33680.32001" target="_blank">10.13140/RG.2.2.33680.32001</a></p>
        </span>
      </p>
      <p>
        <span class="lang-en">
          I have developed strong expertise in bioinformatics and omics data analysis, combining computational tools with advanced statistical methods. My experience includes programming in R and Python, machine learning applied to biomedical data, multivariate analysis, and statistical modeling.
        </span>
      </p>
      <p>
        <span class="lang-en">
          I have worked with transcriptomics, genomics, and other high-throughput data, applying predictive models and statistical inference to extract meaningful insights. Additionally, I am proficient in specialized software for biomedical data analysis and omics data integration techniques.
          Master's Thesis: Identification and characterization of overexpressed tRFs in Huntington's disease. DOI: 
          <a href="https://doi.org/10.13140/RG.2.2.33680.32001" target="_blank">10.13140/RG.2.2.33680.32001</a>
        </span>
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
      <!-- Versión en español -->
      <div class="lang-es">
        <p>
          He adquirido una sólida base en genética molecular y citología, con conocimientos en estructura y función de los genomas, biología celular, embriología y técnicas avanzadas de laboratorio. Además, tengo experiencia en la caracterización estructural de genes, análisis genético en protistas y aplicación de métodos de laboratorio en anatomía patológica y citología.
        </p>
        <p>
          TFG: Caracterización estructural de genes codificantes de proteínas ribosómicas en Leishmania. DOI: 
          <a href="https://doi.org/10.13140/RG.2.2.10192.21767" target="_blank">10.13140/RG.2.2.10192.21767</a>.
        </p>
        <p>
          Participación mencionada en el 
          <a href="https://www.cbm.uam.es/wp-content/uploads/2024/07/CBM-Scientific-Report-2021-2022.pdf" target="_blank">
            Informe Científico del CBMSO-CSIC 2021–2022
          </a>.
        </p>
      </div>
      
      <!-- Versión en inglés -->
      <div class="lang-en">
        <p>
          I have developed a strong foundation in molecular genetics and cytology, with expertise in genome structure and function, cell biology, embryology, and advanced laboratory techniques. Additionally, I have experience in gene structural characterization, genetic analysis in protists, and laboratory methods in pathological anatomy and cytology.
        </p>
        <p>
          Bachelor's Thesis: Structural characterization of genes coding for ribosomal proteins in Leishmania. DOI: 
          <a href="https://doi.org/10.13140/RG.2.2.10192.21767" target="_blank">10.13140/RG.2.2.10192.21767</a>.
        </p>
        <p>
          Participation mentioned in the 
          <a href="https://www.cbm.uam.es/wp-content/uploads/2024/07/CBM-Scientific-Report-2021-2022.pdf" target="_blank">
            CBMSO-CSIC Scientific Report 2021–2022
          </a>.
        </p>
      </div>
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
        <span class="lang-es">
          Detección Inmunohistoquímica de BRCA en Cáncer de Mama<br><br>
          En este proyecto, realicé la detección inmunohistoquímica de los genes BRCA1 y BRCA2 en muestras de tejido mamario con sospecha de cáncer. Utilicé anticuerpos específicos para BRCA y otros marcadores como HER2, Ki-67, ER y PR. Tras aplicar los anticuerpos, se visualizó la expresión de BRCA en las células mediante un marcador cromogénico (DAB), que generó manchas marrones en las células positivas.<br><br>
          Este proyecto me permitió desarrollar habilidades en técnicas de inmunohistoquímica, microscopía y la interpretación de marcadores tumorales en la investigación del cáncer de mama.
        </span>
        <span class="lang-en">
          Immunohistochemical Detection of BRCA in Breast Cancer<br><br>
          In this project, I performed the immunohistochemical detection of BRCA1 and BRCA2 genes in breast tissue samples with suspected cancer. I used specific antibodies for BRCA, as well as other markers such as HER2, Ki-67, ER, and PR. After applying the antibodies, the expression of BRCA in the cells was visualized through a chromogenic marker (DAB), which produced brown spots in the positive cells.<br><br>
          This project allowed me to develop skills in immunohistochemical techniques, microscopy, and tumor marker interpretation in breast cancer research.
        </span>
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
<!-- Sección: Autorreflexión -->
<section id="autorreflexion-section" class="direct-section">
  <h2 class="section-title">
    <span class="lang-es">🧠 Autorreflexión sobre mi proceso de aprendizaje</span>
    <span class="lang-en">🧠 Self-reflection on my learning process</span>
  </h2>
  <p>
    <span class="lang-es">A lo largo de mi carrera académica y profesional, he tenido la oportunidad de integrar mis conocimientos en biología, bioinformática, robótica y visión computacional 3D. Esta combinación interdisciplinaria ha sido clave para mi desarrollo, tanto como investigadora predoctoral en la UPM y CRF-INIA-CSIC como en mis estudios anteriores en el grado de Biología y el máster en Bioinformática.</span>
    <span class="lang-en">Throughout my academic and professional career, I have had the opportunity to integrate my knowledge in biology, bioinformatics, robotics, and 3D computer vision. This interdisciplinary combination has been key to my development, both as a predoctoral researcher at UPM and CRF-INIA-CSIC and in my previous studies in Biology and the master's degree in Bioinformatics.</span>
  </p>
  <p>
    <span class="lang-es">Mi primer contacto con la investigación fue en 1º de Bachillerato, cuando desarrollé un proyecto sobre la síntesis de bioplásticos a partir de la leche de vaca. Ese primer acercamiento a la ciencia me motivó a seguir explorando más en profundidad, y me permitió darme cuenta de lo fascinante que es la capacidad de hacer avanzar el conocimiento a través de la investigación. Desde entonces, cada paso en mi trayectoria ha sido una oportunidad de aprender y mejorar.</span>
    <span class="lang-en">My first contact with research was in the first year of high school when I developed a project on the synthesis of bioplastics from cow's milk. This first approach to science motivated me to continue exploring more deeply and made me realize how fascinating it is to advance knowledge through research. Since then, every step in my journey has been an opportunity to learn and improve.</span>
  </p>
  <p>
    <span class="lang-es">A medida que he ido avanzando en mis estudios y proyectos, he aprendido a integrar herramientas y enfoques de diferentes disciplinas. En mis investigaciones actuales, por ejemplo, he logrado combinar mis conocimientos en biología con las técnicas de visión computacional y robótica para resolver problemas complejos, como el fenotipado automatizado de cultivos. La programación en Python y R, así como el uso de técnicas de machine learning, han sido fundamentales para poder procesar y analizar grandes volúmenes de datos.</span>
    <span class="lang-en">As I have progressed in my studies and projects, I have learned to integrate tools and approaches from different disciplines. In my current research, for example, I have been able to combine my knowledge of biology with computer vision and robotics techniques to solve complex problems, such as the automated phenotyping of crops. Programming in Python and R, as well as using machine learning techniques, have been essential for processing and analyzing large datasets.</span>
  </p>
  <p>
    <span class="lang-es">Una de las cosas que he aprendido sobre mí misma es que soy capaz de abordar proyectos complejos y multidisciplinarios, pero también he identificado áreas en las que necesito mejorar. Por ejemplo, la gestión del tiempo sigue siendo un reto, sobre todo cuando estoy involucrada en varios proyectos a la vez. A veces es difícil equilibrar todas las tareas que tengo, y eso me ha llevado a buscar maneras de organizarme mejor y priorizar de manera más eficaz. También, aunque me siento cómoda usando herramientas estadísticas avanzadas, me gustaría mejorar mi capacidad para comunicar mis resultados de manera clara y comprensible, tanto para compañeros de mi campo como para aquellos ajenos a la ciencia.</span>
    <span class="lang-en">One thing I have learned about myself is that I am capable of tackling complex and multidisciplinary projects, but I have also identified areas where I need to improve. For example, time management remains a challenge, especially when I am involved in several projects at once. It is sometimes difficult to balance all the tasks I have, and this has led me to look for better ways to organize myself and prioritize more effectively. Also, although I feel comfortable using advanced statistical tools, I would like to improve my ability to communicate my results clearly and understandably, both to peers in my field and to those outside of science.</span>
  </p>
  <p>
    <span class="lang-es">Mirando hacia el futuro, mi objetivo es seguir desarrollando mis habilidades en áreas como la inteligencia artificial y la robótica, especialmente aplicadas a la biología y la agricultura. Además, quiero seguir reflexionando sobre mi proceso de aprendizaje para poder mejorar continuamente, ajustando mis métodos de trabajo y mis estrategias de estudio.</span>
    <span class="lang-en">Looking ahead, my goal is to continue developing my skills in areas such as artificial intelligence and robotics, especially applied to biology and agriculture. In addition, I want to continue reflecting on my learning process to keep improving, adjusting my work methods and study strategies.</span>
  </p>
  <p>
    <span class="lang-es">En resumen, este ejercicio de autorreflexión me ha permitido darme cuenta de cuánto he avanzado y de lo que todavía puedo mejorar. Creo que es fundamental seguir reflexionando sobre el aprendizaje para poder adaptarse a los desafíos que vienen, y estoy muy motivada para seguir creciendo profesional y personalmente.</span>
    <span class="lang-en">In summary, this self-reflection exercise has allowed me to realize how much I have progressed and what I still need to improve. I believe it is essential to keep reflecting on learning in order to adapt to the challenges ahead, and I am very motivated to keep growing both professionally and personally.</span>
  </p>
</section>

<!-- Sección: Contacto -->
<section id="contacto-section" class="direct-section">
  <h2 class="section-title">
    <span class="lang-es">📫 Contacto</span>
    <span class="lang-en">📫 Contact</span>
  </h2>
  <ul>
    <li><span class="lang-es">📖 ResearchGate:</span><span class="lang-en">📖 ResearchGate:</span> <a href="https://www.researchgate.net/profile/Andrea-Clemente-Urena-2">Andrea-Clemente-Urena-2</a></li>
    <li><span class="lang-es">🔗 LinkedIn:</span><span class="lang-en">🔗 LinkedIn:</span> <a href="https://www.linkedin.com/in/andreaclementeure%C3%B1a/" target="_blank">linkedin.com/in/andreaclementeureña</a></li>
    <li><span class="lang-es">💻 GitHub:</span><span class="lang-en">💻 GitHub:</span> <a href="https://github.com/andreaclemente96" target="_blank">andreaclemente96</a></li>
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
  <div class="footer-text" id="image-credits">
    <span class="lang-es">Imágenes utilizadas: Propias o de <a href="https://www.freepik.es/imagenes" target="_blank">Freepik</a> bajo licencia de uso libre.</span>
    <span class="lang-en">Images used: Owned or from <a href="https://www.freepik.es/imagenes" target="_blank">Freepik</a> under a free-use license. </span>
  </div>
  
</footer>

<script type="text/javascript" src="https://cdn.emailjs.com/dist/email.min.js"></script>
<script>
  //  DOM
  document.addEventListener('DOMContentLoaded', function() {
    // Inicializa EmailJS con tu User ID
    emailjs.init('c-V5Vr4aJmeXBnuYI'); 

    // Evento del formulario
    document.getElementById("contact-form").addEventListener("submit", function(e) {
      e.preventDefault();
      console.log("Submit del formulario detectado");
      
      // Enviar el formulario usando EmailJS
      emailjs.sendForm('Andrea_gmail', 'template_9te72ls', this)
        .then(function(response) {
          console.log("Respuesta de EmailJS:", response);
          alert(
            document.documentElement.lang === 'es' 
              ? "Formulario enviado. Gracias por tu mensaje." 
              : "Form submitted. Thank you for your message."
          );
          document.getElementById("contact-form").reset();
        }, function(error) {
          console.error("Error en EmailJS:", error);
          alert(
            document.documentElement.lang === 'es' 
              ? "Hubo un error al enviar el mensaje. Intenta de nuevo."
              : "There was an error sending the message. Please try again."
          );
        });
    });

    // Detectar el idioma del navegador 
    const browserLanguage = navigator.language || navigator.userLanguage;
    const html = document.documentElement;
    if (browserLanguage.startsWith('es')) {
      html.lang = 'es';
      document.getElementById("language-toggle").innerText = "English";
    } else {
      html.lang = 'en';
      document.getElementById("language-toggle").innerText = "Español";
    }

    // Mostrar los elementos según el idioma establecido
    const esElements = document.querySelectorAll('.lang-es');
    const enElements = document.querySelectorAll('.lang-en');
    if (html.lang === 'es') {
      esElements.forEach(el => el.style.display = 'inline');
      enElements.forEach(el => el.style.display = 'none');
    } else {
      esElements.forEach(el => el.style.display = 'none');
      enElements.forEach(el => el.style.display = 'inline');
    }
  });

  // Función para cambiar de idioma (al hacer clic en el botón)
  function toggleLanguage() {
    const html = document.documentElement;
    const isEnglish = html.lang === 'en';
    html.lang = isEnglish ? 'es' : 'en';
    document.getElementById("language-toggle").innerText = isEnglish ? "English" : "Español";
    
    const esElements = document.querySelectorAll('.lang-es');
    const enElements = document.querySelectorAll('.lang-en');
    if (html.lang === 'es') {
      esElements.forEach(el => el.style.display = 'inline');
      enElements.forEach(el => el.style.display = 'none');
    } else {
      esElements.forEach(el => el.style.display = 'none');
      enElements.forEach(el => el.style.display = 'inline');
    }
  }

  document.querySelectorAll('.project-image').forEach(project => {
    project.addEventListener('click', () => {
      const description = project.closest('.project-container').querySelector('.project-description');
      description.classList.toggle('active');
    });
  });
</script>
</body>
</html>

