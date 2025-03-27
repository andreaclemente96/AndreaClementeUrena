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
    }
    h1, h2, h3 {
      color: #2c3e50;
    }
    header {
      text-align: center;
      margin-bottom: 2rem;
    }
    img {
      max-width: 100%;
      height: auto;
      border-radius: 10px;
      margin: 1rem 0;
      cursor: pointer;
    }
    .grid {
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      justify-content: center;
    }
    .grid img {
      max-width: 45%;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin: 1rem 0;
    }
    td, th {
      padding: 0.5rem;
    }
    tr:nth-child(even) {
      background-color: #eaf0f7;
    }
    .center-img {
      display: block;
      margin: 1rem auto;
      max-width: 400px;
    }
    footer {
      text-align: center;
      margin-top: 2rem;
      font-style: italic;
      color: #555;
    }
    .content {
      display: none;
      margin-top: 10px;
    }
    .section-header {
      cursor: pointer;
      margin-top: 20px;
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
    }
    /* Estilos para el formulario de contacto */
    form {
      margin-top: 2rem;
      background-color: #eef4fa;
      padding: 1rem;
      border-radius: 10px;
      max-width: 600px;
      margin-left: auto;
      margin-right: auto;
    }
    form label {
      display: block;
      margin-top: 1rem;
    }
    form input, form textarea {
      width: 100%;
      padding: 8px;
      margin-top: 8px;
      margin-bottom: 16px;
      border: 1px solid #ccc;
      border-radius: 4px;
    }
    form input[type="submit"] {
      background-color: #2c3e50;
      color: white;
      cursor: pointer;
      border: none;
      padding: 10px 15px;
    }
    /* Traducción: inicialmente mostramos el español y ocultamos el inglés */
    .lang-en { display: none; }
  </style>
</head>
<body>

<!-- Botón para alternar el idioma -->
<button id="language-toggle" onclick="toggleLanguage()">English</button>

<header>
  <h1>
    <span class="lang-es">👩‍🔬 Andrea Clemente-Ureña</span>
    <span class="lang-en">👩‍🔬 Andrea Clemente-Ureña</span>
  </h1>
  <p>
    <span class="lang-es"> Aquí comparto mi trayectoria en <strong>biología</strong>, <strong>bioinformática</strong>, <strong>robótica</strong> y <strong>visión computacional 3D</strong>.</span>
    <span class="lang-en">Here I share my journey in <strong>biology</strong>, <strong>bioinformatics</strong>, <strong>robotics</strong> and <strong>3D computer vision</strong>.</span>
  </p>
  <p>
    <span class="lang-es"><strong>Investigadora predoctoral</strong> en UPM y CRF-INIA-CSIC | Proyecto: Transformación digital de la conservación y mejora vegetal</span>
    <span class="lang-en"><strong>Predoctoral Researcher</strong> at UPM and CRF-INIA-CSIC | Project: Digital Transformation of Plant Conservation and Improvement</span>
  </p>
</header>

<!-- Sección: Bienvenida (siempre visible) -->
<section>
  <h2>
    <span class="lang-es">¡Bienvenid@ a mi portfolio!</span>
    <span class="lang-en">Welcome to my portfolio!</span>
  </h2>
  <div>
    <p>
      <span class="lang-es">Este espacio reúne mi trayectoria en <strong>biología</strong>, <strong>bioinformática</strong>, <strong>robótica</strong> y <strong>visión computacional 3D</strong>. Actualmente desarrollo herramientas avanzadas para el <strong>fenotipado de cultivos</strong> y la <strong>caracterización de estructuras vegetales</strong>, aplicando aprendizaje automático y análisis de datos.</span>
      <span class="lang-en">This space brings together my journey in <strong>biology</strong>, <strong>bioinformatics</strong>, <strong>robotics</strong>, and <strong>3D computer vision</strong>. I currently develop advanced tools for <strong>crop phenotyping</strong> and <strong>plant structure characterization</strong> using machine learning and data analysis.</span>
    </p>
    <p>
      <span class="lang-es">📍 Investigadora predoctoral en la Universidad Politécnica de Madrid (UPM) y el Centro de Recursos Fitogenéticos (CRF-INIA-CSIC), dentro del proyecto <strong>Transformación digital de las actividades de conservación y mejora vegetal</strong>.</span>
      <span class="lang-en">📍 Predoctoral researcher at the Polytechnic University of Madrid (UPM) and the Fitogenetic Resources Center (CRF-INIA-CSIC), in the project <strong>Digital Transformation of Plant Conservation and Improvement</strong>.</span>
    </p>
  </div>
</section>

<!-- Sección: Mi primer contacto con la investigación -->
<section>
  <h2 class="section-header" onclick="toggleContent('primer_contacto')">
    <span class="lang-es">💡 Mi primer contacto con la investigación</span>
    <span class="lang-en">💡 My First Encounter with Research</span>
  </h2>
  <!-- Imagen actualizada; si no se muestra, revisa la URL en el navegador -->
  <img src="https://img.freepik.com/foto-gratis/2147654639.jpg" alt="Mi primer contacto con la investigación" onclick="toggleContent('primer_contacto')">
  <div id="primer_contacto" class="content">
    <p>
      <span class="lang-es">Mi primer contacto con la investigación fue en 1º de Bachillerato, cuando desarrollé un proyecto sobre la <em>síntesis de bioplásticos a partir de la leche de vaca</em> en las asignaturas de Biología y Técnicas Experimentales en Ciencias. Ese mismo año participé en el <strong>Finde Científico</strong>, formando parte de un equipo que realizaba experimentos de química visual (cambio de color gracias a las reacciones) para la divulgación científica, diseñados para acercar la ciencia a estudiantes, niños y familias en general.</span>
      <span class="lang-en">My first encounter with research was in the first year of high school when I developed a project on the <em>synthesis of bioplastics from cow's milk</em> in Biology and Experimental Techniques classes. That same year, I participated in Finde Científico, as part of a team performing visual chemistry experiments (color changes due to reactions) to bring science closer to students, children, and families.</span>
    </p>
    <div style="display: flex; justify-content: center; gap: 20px;">
      <img src="https://github.com/user-attachments/assets/2507bf89-76fb-4903-b5fb-6aea3606fc46" alt="Síntesis de bioplásticos a partir de la leche de vaca" width="300">
      <img src="https://github.com/user-attachments/assets/fda0a450-37c9-4553-8ba1-94f0d26d670c" alt="Finde Científico: Experimentos de química visual" width="300">
    </div>
  </div>
</section>

<!-- Sección: Proyectos destacados -->
<section>
  <h2 class="section-header" onclick="toggleContent('proyectos')">
    <span class="lang-es">🚀 Proyectos destacados</span>
    <span class="lang-en">🚀 Featured Projects</span>
  </h2>
  <img src="https://via.placeholder.com/400x200?text=Proyectos" alt="Imagen Proyectos" onclick="toggleContent('proyectos')">
  <div id="proyectos" class="content">
    <ul>
      <li>
        <strong>
          <span class="lang-es">Fenotipado de alto rendimiento</span>
          <span class="lang-en">High-performance Phenotyping</span>
        </strong>
        <ul>
          <li>
            <span class="lang-es">Integración de sensores RGB, multiespectrales y LiDAR en robots autónomos.</span>
            <span class="lang-en">Integration of RGB, multispectral, and LiDAR sensors on autonomous robots.</span>
          </li>
          <li>
            <span class="lang-es">Procesamiento de datos 3D y modelos de IA para el análisis de cultivos.</span>
            <span class="lang-en">3D data processing and AI models for crop analysis.</span>
          </li>
        </ul>
        <p align="center">
          <img src="https://github.com/user-attachments/assets/9905699f-ddda-4b6a-970a-08e2fbd359aa" alt="Fenotipado de alto rendimiento" width="400">
        </p>
      </li>
      <li>
        <strong>
          <span class="lang-es">Bioinformática y análisis ómico</span>
          <span class="lang-en">Bioinformatics and Omics Analysis</span>
        </strong>
        <ul>
          <li>
            <span class="lang-es">TFM: <em>Identificación y caracterización de tRFs sobreexpresados en enfermedad de Huntington</em>.</span>
            <span class="lang-en">Master's Thesis: <em>Identification and characterization of overexpressed tRFs in Huntington’s disease</em>.</span>
          </li>
          <li>📄 DOI: <a href="https://doi.org/10.13140/RG.2.2.33680.32001" target="_blank">10.13140/RG.2.2.33680.32001</a></li>
        </ul>
        <p align="center">
          <img src="https://github.com/user-attachments/assets/8dfa2628-f892-4078-bde3-3915150bed34" alt="Bioinformática y análisis ómico" width="400">
        </p>
      </li>
      <li>
        <strong>
          <span class="lang-es">Genética molecular y citología</span>
          <span class="lang-en">Molecular Genetics and Cytology</span>
        </strong>
        <ul>
          <li>
            <span class="lang-es">TFG: <em>Caracterización estructural de genes codificantes de proteínas ribosómicas en Leishmania</em>.</span>
            <span class="lang-en">Bachelor’s Thesis: <em>Structural characterization of genes coding for ribosomal proteins in Leishmania</em>.</span>
          </li>
          <li>📄 DOI: <a href="https://doi.org/10.13140/RG.2.2.10192.21767" target="_blank">10.13140/RG.2.2.10192.21767</a></li>
          <li>
            <span class="lang-es">📰 Participación mencionada en el <a href="https://www.cbm.uam.es/wp-content/uploads/2024/07/CBM-Scientific-Report-2021-2022.pdf" target="_blank">Informe Científico del CBMSO-CSIC 2021–2022</a></span>
            <span class="lang-en">📰 Participation mentioned in the <a href="https://www.cbm.uam.es/wp-content/uploads/2024/07/CBM-Scientific-Report-2021-2022.pdf" target="_blank">CBMSO-CSIC Scientific Report 2021–2022</a></span>
          </li>
        </ul>
        <p align="center">
          <img src="https://github.com/user-attachments/assets/b740f460-1160-4a35-90c6-b3b2e5861f23" alt="Genética molecular y citología" width="400">
        </p>
      </li>
      <li>
        <strong>
          <span class="lang-es">Histología e inmunohistoquímica</span>
          <span class="lang-en">Histology and Immunohistochemistry</span>
        </strong>
        <ul>
          <li>
            <span class="lang-es">Proyecto sobre detección inmunohistoquímica de BRCA en cáncer de mama durante el FPII.</span>
            <span class="lang-en">Project on immunohistochemical detection of BRCA in breast cancer during FPII.</span>
          </li>
        </ul>
        <p align="center">
          <img src="https://github.com/user-attachments/assets/73e74b49-a323-40f3-b055-1f3bfaf9750c" alt="Histología e inmunohistoquímica" width="400">
        </p>
      </li>
      <li>
        <strong>
          <span class="lang-es">Exploración con tecnologías inmersivas</span>
          <span class="lang-en">Exploration with Immersive Technologies</span>
        </strong>
        <ul>
          <li>
            <span class="lang-es">Colaboración con el <strong>Centro de Automática y Robótica (CAR-CSIC-UPM)</strong> para desarrollar soluciones con <strong>Microsoft HoloLens2</strong> en aplicaciones agrícolas. <em>(Proyecto en fase inicial)</em></span>
            <span class="lang-en">Collaboration with the <strong>Center for Automation and Robotics (CAR-CSIC-UPM)</strong> to develop solutions with <strong>Microsoft HoloLens2</strong> in agricultural applications. <em>(Initial project)</em></span>
          </li>
        </ul>
      </li>
    </ul>
  </div>
</section>

<!-- Sección: Formación académica -->
<section>
  <h2 class="section-header" onclick="toggleContent('formacion')">
    <span class="lang-es">🎓 Formación académica</span>
    <span class="lang-en">🎓 Academic Background</span>
  </h2>
  <img src="https://via.placeholder.com/400x200?text=Formaci%C3%B3n" alt="Imagen Formación" onclick="toggleContent('formacion')">
  <div id="formacion" class="content">
    <ul>
      <li>
        <span class="lang-es">📘 <strong>Doctorado en Automática y Robótica</strong> (2024 - actualidad) - Universidad Politécnica de Madrid – INIA-CSIC</span>
        <span class="lang-en">📘 <strong>PhD in Automation and Robotics</strong> (2024 - Present) - Polytechnic University of Madrid – INIA-CSIC</span>
      </li>
      <li>
        <span class="lang-es">📊 <strong>Máster en Bioinformática y Bioestadística</strong> (2022 - 2024) - Universitat Oberta de Catalunya / Universitat de Barcelona</span>
        <span class="lang-en">📊 <strong>Master in Bioinformatics and Biostatistics</strong> (2022 - 2024) - Open University of Catalonia / University of Barcelona</span>
      </li>
      <li>
        <span class="lang-es">🧬 <strong>Grado en Biología</strong> (2016 - 2021) - Universidad Autónoma de Madrid</span>
        <span class="lang-en">🧬 <strong>Bachelor in Biology</strong> (2016 - 2021) - Autonomous University of Madrid</span>
      </li>
      <li>
        <span class="lang-es">🔬 <strong>Técnico Superior en Anatomía Patológica y Citología</strong> (2014 - 2016) - CESUR II</span>
        <span class="lang-en">🔬 <strong>Higher Technician in Pathological Anatomy and Cytology</strong> (2014 - 2016) - CESUR II</span>
      </li>
    </ul>
  </div>
</section>

<!-- Sección: Tecnologías y herramientas -->
<section>
  <h2 class="section-header" onclick="toggleContent('tecnologias')">
    <span class="lang-es">🛠️ Tecnologías y herramientas</span>
    <span class="lang-en">🛠️ Technologies &amp; Tools</span>
  </h2>
  <img src="https://via.placeholder.com/400x200?text=Tecnolog%C3%ADas" alt="Imagen Tecnologías" onclick="toggleContent('tecnologias')">
  <div id="tecnologias" class="content">
    <table>
      <tr>
        <td><strong>
          <span class="lang-es">Lenguajes</span>
          <span class="lang-en">Languages</span>
        </strong></td>
        <td>Python • R • SQL • BASH • HTML/CSS</td>
      </tr>
      <tr>
        <td><strong>
          <span class="lang-es">Ciencia &amp; Bioinfo</span>
          <span class="lang-en">Science &amp; Bioinformatics</span>
        </strong></td>
        <td>Bioconductor • SPSS • Galaxy • Novopath • Inferencia estadística</td>
      </tr>
      <tr>
        <td><strong>
          <span class="lang-es">IA / Visión</span>
          <span class="lang-en">AI / Vision</span>
        </strong></td>
        <td>OpenCV • PyTorch • TensorFlow • Scikit-learn • Visión 3D</td>
      </tr>
      <tr>
        <td><strong>
          <span class="lang-es">Robótica</span>
          <span class="lang-en">Robotics</span>
        </strong></td>
        <td>Sensores RGB • Sensores Multiespectrales • Sensores LiDAR/ToF • HoloLens 2</td>
      </tr>
      <tr>
        <td><strong>
          <span class="lang-es">Entornos</span>
          <span class="lang-en">Environments</span>
        </strong></td>
        <td>Linux • VS Code • Git • Office</td>
      </tr>
    </table>
  </div>
</section>

<!-- Sección: Experiencia profesional -->
<section>
  <h2 class="section-header" onclick="toggleContent('experiencia')">
    <span class="lang-es">📚 Experiencia profesional</span>
    <span class="lang-en">📚 Professional Experience</span>
  </h2>
  <img src="https://via.placeholder.com/400x200?text=Experiencia" alt="Imagen Experiencia" onclick="toggleContent('experiencia')">
  <div id="experiencia" class="content">
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
  </div>
</section>

<!-- Sección: Idiomas -->
<section>
  <h2 class="section-header" onclick="toggleContent('idiomas')">
    <span class="lang-es">🌐 Idiomas</span>
    <span class="lang-en">🌐 Languages</span>
  </h2>
  <img src="https://via.placeholder.com/400x200?text=Idiomas" alt="Imagen Idiomas" onclick="toggleContent('idiomas')">
  <div id="idiomas" class="content">
    <ul>
      <li><span class="lang-es">🇪🇸 Español: Nativo</span><span class="lang-en">🇪🇸 Spanish: Native</span></li>
      <li><span class="lang-es">🇬🇧 Inglés: Nivel C (APTIS - British Council)</span><span class="lang-en">🇬🇧 English: Level C (APTIS - British Council)</span></li>
      <li><span class="lang-es">🇫🇷 Francés: Nivel A2 (DELF)</span><span class="lang-en">🇫🇷 French: Level A2 (DELF)</span></li>
    </ul>
  </div>
</section>

<!-- Sección: Contacto (datos) -->
<section>
  <h2 class="section-header" onclick="toggleContent('contacto')">
    <span class="lang-es">📫 Contacto</span>
    <span class="lang-en">📫 Contact</span>
  </h2>
  <img src="https://via.placeholder.com/400x200?text=Contacto" alt="Imagen Contacto" onclick="toggleContent('contacto')">
  <div id="contacto" class="content">
    <ul>
      <li><span class="lang-es">✉️ Email:</span><span class="lang-en">✉️ Email:</span> <a href="mailto:andeande.ac@gmail.com">andeande.ac@gmail.com</a></li>
      <li><span class="lang-es">🔗 LinkedIn:</span><span class="lang-en">🔗 LinkedIn:</span> <a href="https://www.linkedin.com/in/andreaclementeure%C3%B1a/" target="_blank">https://www.linkedin.com/in/andreaclementeure%C3%B1a/</a></li>
      <li><span class="lang-es">💻 GitHub:</span><span class="lang-en">💻 GitHub:</span> <a href="https://github.com/andyacment" target="_blank">https://github.com/andyacment</a></li>
    </ul>
  </div>
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
  <textarea id="message" name="message" rows="5" required></textarea>
  <input type="submit" value="Enviar">
</form>

<footer>
  <p>
    <span class="lang-es">_"La IA no es el enemigo, es la lupa que amplifica lo que la ciencia aún no alcanza."_ 🤖🔬🌍</span>
    <span class="lang-en">_"AI is not the enemy; it is the magnifying glass that amplifies what science has not yet reached."_ 🤖🔬🌍</span>
  </p>
</footer>

<script>
  function toggleContent(id) {
    var content = document.getElementById(id);
    content.style.display = content.style.display === "block" ? "none" : "block";
  }

  function toggleLanguage() {
    // Si el idioma actual es español, ocultamos los elementos lang-es y mostramos lang-en, y viceversa.
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

  // Manejador del envío del formulario (solo front-end)
  document.getElementById("contact-form").addEventListener("submit", function(e) {
    e.preventDefault();
    alert("Formulario enviado. Gracias por tu mensaje.");
    this.reset();
  });
</script>

</body>
</html>
