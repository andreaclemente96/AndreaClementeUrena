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
  </style>
</head>
<body>

<!-- Botón para alternar el idioma -->
<button id="language-toggle" onclick="toggleLanguage()">English</button>

<header>
  <h1 data-es="👩‍🔬 Andrea Clemente-Ureña" data-en="👩‍🔬 Andrea Clemente-Ureña">👩‍🔬 Andrea Clemente-Ureña</h1>
  <p data-es="Bienvenid@ a mi portfolio. Aquí comparto mi trayectoria en biología, bioinformática, robótica y visión computacional 3D." 
     data-en="Welcome to my portfolio. Here I share my journey in biology, bioinformatics, robotics, and 3D computer vision.">
    Bienvenid@ a mi portfolio. Aquí comparto mi trayectoria en <strong>biología</strong>, <strong>bioinformática</strong>, <strong>robótica</strong> y <strong>visión computacional 3D</strong>.
  </p>
  <p data-es="<strong>Investigadora predoctoral</strong> en UPM y CRF-INIA-CSIC | Proyecto: Transformación digital de la conservación y mejora vegetal" 
     data-en="<strong>Predoctoral Researcher</strong> at UPM and CRF-INIA-CSIC | Project: Digital Transformation of Plant Conservation and Improvement">
    <strong>Investigadora predoctoral</strong> en UPM y CRF-INIA-CSIC | Proyecto: Transformación digital de la conservación y mejora vegetal
  </p>
</header>

<!-- Sección: Bienvenida (siempre visible) -->
<section>
  <h2 data-es="¡Bienvenid@ a mi portfolio!" data-en="Welcome to my portfolio!">¡Bienvenid@ a mi portfolio!</h2>
  <div>
    <p data-es="Este espacio reúne mi trayectoria en biología, bioinformática, robótica y visión computacional 3D. Actualmente desarrollo herramientas avanzadas para el fenotipado de cultivos y la caracterización de estructuras vegetales, aplicando aprendizaje automático y análisis de datos." 
       data-en="This space brings together my journey in biology, bioinformatics, robotics, and 3D computer vision. I currently develop advanced tools for crop phenotyping and plant structure characterization using machine learning and data analysis.">
      Este espacio reúne mi trayectoria en <strong>biología</strong>, <strong>bioinformática</strong>, <strong>robótica</strong> y <strong>visión computacional 3D</strong>. Actualmente desarrollo herramientas avanzadas para el <strong>fenotipado de cultivos</strong> y la <strong>caracterización de estructuras vegetales</strong>, aplicando aprendizaje automático y análisis de datos.
    </p>
    <p data-es="📍 Investigadora predoctoral en la Universidad Politécnica de Madrid (UPM) y el Centro de Recursos Fitogenéticos (CRF-INIA-CSIC), dentro del proyecto Transformación digital de las actividades de conservación y mejora vegetal." 
       data-en="📍 Predoctoral researcher at the Polytechnic University of Madrid (UPM) and the Fitogenetic Resources Center (CRF-INIA-CSIC), in the project Digital Transformation of Plant Conservation and Improvement.">
      📍 Investigadora predoctoral en la Universidad Politécnica de Madrid (UPM) y el Centro de Recursos Fitogenéticos (CRF-INIA-CSIC), dentro del proyecto <strong>Transformación digital de las actividades de conservación y mejora vegetal</strong>.
    </p>
  </div>
</section>

<!-- Sección: Mi primer contacto con la investigación -->
<section>
  <h2 class="section-header" 
      data-es="💡 Mi primer contacto con la investigación" 
      data-en="💡 My First Encounter with Research" 
      onclick="toggleContent('primer_contacto')">
    💡 Mi primer contacto con la investigación
  </h2>
  <!-- Imagen actualizada -->
  <img src="https://img.freepik.com/foto-gratis/lapices-compuestos-pizarra_1313812.jpg" alt="Mi primer contacto con la investigación" onclick="toggleContent('primer_contacto')">
  <div id="primer_contacto" class="content">
    <p data-es="Mi primer contacto con la investigación fue en 1º de Bachillerato, cuando desarrollé un proyecto sobre la síntesis de bioplásticos a partir de la leche de vaca en las asignaturas de Biología y Técnicas Experimentales en Ciencias. Ese mismo año participé en el Finde Científico, formando parte de un equipo que realizaba experimentos de química visual (cambio de color gracias a las reacciones) para la divulgación científica, diseñados para acercar la ciencia a estudiantes, niños y familias en general." 
       data-en="My first encounter with research was in the first year of high school when I developed a project on synthesizing bioplastics from cow's milk in Biology and Experimental Techniques classes. That same year, I participated in Finde Científico, as part of a team conducting visual chemistry experiments (color changes due to reactions) to bring science closer to students, children, and families.">
      Mi primer contacto con la investigación fue en 1º de Bachillerato, cuando desarrollé un proyecto sobre la <strong>síntesis de bioplásticos a partir de la leche de vaca</strong> en las asignaturas de Biología y Técnicas Experimentales en Ciencias. Ese mismo año participé en el <strong>Finde Científico</strong>, formando parte de un equipo que realizaba experimentos de química visual (cambio de color gracias a las reacciones) para la divulgación científica, diseñados para acercar la ciencia a estudiantes, niños y familias en general.
    </p>
    <div style="display: flex; justify-content: center; gap: 20px;">
      <img src="https://github.com/user-attachments/assets/2507bf89-76fb-4903-b5fb-6aea3606fc46" alt="Síntesis de bioplásticos a partir de la leche de vaca" width="300">
      <img src="https://github.com/user-attachments/assets/fda0a450-37c9-4553-8ba1-94f0d26d670c" alt="Finde Científico: Experimentos de química visual" width="300">
    </div>
  </div>
</section>

<!-- Sección: Proyectos destacados -->
<section>
  <h2 class="section-header" 
      data-es="🚀 Proyectos destacados" 
      data-en="🚀 Featured Projects" 
      onclick="toggleContent('proyectos')">
    🚀 Proyectos destacados
  </h2>
  <img src="https://via.placeholder.com/400x200?text=Proyectos" alt="Imagen Proyectos" onclick="toggleContent('proyectos')">
  <div id="proyectos" class="content">
    <ul>
      <li>
        <strong data-es="Fenotipado de alto rendimiento" data-en="High-performance Phenotyping">Fenotipado de alto rendimiento</strong>
        <ul>
          <li data-es="Integración de sensores RGB, multiespectrales y LiDAR en robots autónomos." 
              data-en="Integration of RGB, multispectral, and LiDAR sensors on autonomous robots.">
            Integración de sensores RGB, multiespectrales y LiDAR en robots autónomos.
          </li>
          <li data-es="Procesamiento de datos 3D y modelos de IA para el análisis de cultivos." 
              data-en="3D data processing and AI models for crop analysis.">
            Procesamiento de datos 3D y modelos de IA para el análisis de cultivos.
          </li>
        </ul>
        <p align="center">
          <img src="https://github.com/user-attachments/assets/9905699f-ddda-4b6a-970a-08e2fbd359aa" alt="Fenotipado de alto rendimiento" width="400">
        </p>
      </li>
      <li>
        <strong data-es="Bioinformática y análisis ómico" data-en="Bioinformatics and Omics Analysis">Bioinformática y análisis ómico</strong>
        <ul>
          <li data-es="TFM: Identificación y caracterización de tRFs sobreexpresados en enfermedad de Huntington." 
              data-en="Master's Thesis: Identification and characterization of overexpressed tRFs in Huntington’s disease.">
            TFM: <em>Identificación y caracterización de tRFs sobreexpresados en enfermedad de Huntington</em>.
          </li>
          <li>📄 DOI: <a href="https://doi.org/10.13140/RG.2.2.33680.32001" target="_blank">10.13140/RG.2.2.33680.32001</a></li>
        </ul>
        <p align="center">
          <img src="https://github.com/user-attachments/assets/8dfa2628-f892-4078-bde3-3915150bed34" alt="Bioinformática y análisis ómico" width="400">
        </p>
      </li>
      <li>
        <strong data-es="Genética molecular y citología" data-en="Molecular Genetics and Cytology">Genética molecular y citología</strong>
        <ul>
          <li data-es="TFG: Caracterización estructural de genes codificantes de proteínas ribosómicas en Leishmania." 
              data-en="Bachelor’s Thesis: Structural characterization of genes coding for ribosomal proteins in Leishmania.">
            TFG: <em>Caracterización estructural de genes codificantes de proteínas ribosómicas en Leishmania</em>.
          </li>
          <li>📄 DOI: <a href="https://doi.org/10.13140/RG.2.2.10192.21767" target="_blank">10.13140/RG.2.2.10192.21767</a></li>
          <li data-es="Participación mencionada en el Informe Científico del CBMSO-CSIC 2021–2022." 
              data-en="Participation mentioned in the CBMSO-CSIC Scientific Report 2021–2022.">
            📰 Participación mencionada en el <a href="https://www.cbm.uam.es/wp-content/uploads/2024/07/CBM-Scientific-Report-2021-2022.pdf" target="_blank">Informe Científico del CBMSO-CSIC 2021–2022</a>
          </li>
        </ul>
        <p align="center">
          <img src="https://github.com/user-attachments/assets/b740f460-1160-4a35-90c6-b3b2e5861f23" alt="Genética molecular y citología" width="400">
        </p>
      </li>
      <li>
        <strong data-es="Histología e inmunohistoquímica" data-en="Histology and Immunohistochemistry">Histología e inmunohistoquímica</strong>
        <ul>
          <li data-es="Proyecto sobre detección inmunohistoquímica de BRCA en cáncer de mama durante el FPII." 
              data-en="Project on immunohistochemical detection of BRCA in breast cancer during FPII.">
            Proyecto sobre detección inmunohistoquímica de BRCA en cáncer de mama durante el FPII.
          </li>
        </ul>
        <p align="center">
          <img src="https://github.com/user-attachments/assets/73e74b49-a323-40f3-b055-1f3bfaf9750c" alt="Histología e inmunohistoquímica" width="400">
        </p>
      </li>
      <li>
        <strong data-es="Exploración con tecnologías inmersivas" data-en="Exploration with Immersive Technologies">Exploración con tecnologías inmersivas</strong>
        <ul>
          <li data-es="Colaboración con el Centro de Automática y Robótica (CAR-CSIC-UPM) para desarrollar soluciones con Microsoft HoloLens2 en aplicaciones agrícolas. (Proyecto en fase inicial)" 
              data-en="Collaboration with the Center for Automation and Robotics (CAR-CSIC-UPM) to develop solutions with Microsoft HoloLens2 in agricultural applications. (Initial project)">
            Colaboración con el <strong>Centro de Automática y Robótica (CAR-CSIC-UPM)</strong> para desarrollar soluciones con <strong>Microsoft HoloLens2</strong> en aplicaciones agrícolas. <em>(Proyecto en fase inicial)</em>
          </li>
        </ul>
      </li>
    </ul>
  </div>
</section>

<!-- Sección: Formación académica -->
<section>
  <h2 class="section-header" 
      data-es="🎓 Formación académica" 
      data-en="🎓 Academic Background" 
      onclick="toggleContent('formacion')">
    🎓 Formación académica
  </h2>
  <img src="https://via.placeholder.com/400x200?text=Formaci%C3%B3n" alt="Imagen Formación" onclick="toggleContent('formacion')">
  <div id="formacion" class="content">
    <ul>
      <li data-es="📘 Doctorado en Automática y Robótica (2024 - actualidad) - Universidad Politécnica de Madrid – INIA-CSIC" 
          data-en="📘 PhD in Automation and Robotics (2024 - Present) - Polytechnic University of Madrid – INIA-CSIC">
        📘 <strong>Doctorado en Automática y Robótica</strong> (2024 - actualidad) - Universidad Politécnica de Madrid – INIA-CSIC
      </li>
      <li data-es="📊 Máster en Bioinformática y Bioestadística (2022 - 2024) - Universitat Oberta de Catalunya / Universitat de Barcelona" 
          data-en="📊 Master in Bioinformatics and Biostatistics (2022 - 2024) - Open University of Catalonia / University of Barcelona">
        📊 <strong>Máster en Bioinformática y Bioestadística</strong> (2022 - 2024) - Universitat Oberta de Catalunya / Universitat de Barcelona
      </li>
      <li data-es="🧬 Grado en Biología (2016 - 2021) - Universidad Autónoma de Madrid" 
          data-en="🧬 Bachelor in Biology (2016 - 2021) - Autonomous University of Madrid">
        🧬 <strong>Grado en Biología</strong> (2016 - 2021) - Universidad Autónoma de Madrid
      </li>
      <li data-es="🔬 Técnico Superior en Anatomía Patológica y Citología (2014 - 2016) - CESUR II" 
          data-en="🔬 Higher Technician in Pathological Anatomy and Cytology (2014 - 2016) - CESUR II">
        🔬 <strong>Técnico Superior en Anatomía Patológica y Citología</strong> (2014 - 2016) - CESUR II
      </li>
    </ul>
  </div>
</section>

<!-- Sección: Tecnologías y herramientas -->
<section>
  <h2 class="section-header" 
      data-es="🛠️ Tecnologías y herramientas" 
      data-en="🛠️ Technologies & Tools" 
      onclick="toggleContent('tecnologias')">
    🛠️ Tecnologías y herramientas
  </h2>
  <img src="https://via.placeholder.com/400x200?text=Tecnolog%C3%ADas" alt="Imagen Tecnologías" onclick="toggleContent('tecnologias')">
  <div id="tecnologias" class="content">
    <table>
      <tr>
        <td data-es="Lenguajes" data-en="Languages"><strong>Lenguajes</strong></td>
        <td data-es="Python • R • SQL • BASH • HTML/CSS" data-en="Python • R • SQL • BASH • HTML/CSS">Python • R • SQL • BASH • HTML/CSS</td>
      </tr>
      <tr>
        <td data-es="Ciencia &amp; Bioinfo" data-en="Science &amp; Bioinformatics"><strong>Ciencia &amp; Bioinfo</strong></td>
        <td data-es="Bioconductor • SPSS • Galaxy • Novopath • Inferencia estadística" data-en="Bioconductor • SPSS • Galaxy • Novopath • Statistical inference">Bioconductor • SPSS • Galaxy • Novopath • Inferencia estadística</td>
      </tr>
      <tr>
        <td data-es="IA / Visión" data-en="AI / Vision"><strong>IA / Visión</strong></td>
        <td data-es="OpenCV • PyTorch • TensorFlow • Scikit-learn • Visión 3D" data-en="OpenCV • PyTorch • TensorFlow • Scikit-learn • 3D Vision">OpenCV • PyTorch • TensorFlow • Scikit-learn • Visión 3D</td>
      </tr>
      <tr>
        <td data-es="Robótica" data-en="Robotics"><strong>Robótica</strong></td>
        <td data-es="Sensores RGB • Sensores Multiespectrales • Sensores LiDAR/ToF • HoloLens 2" data-en="RGB Sensors • Multispectral Sensors • LiDAR/ToF Sensors • HoloLens 2">Sensores RGB • Sensores Multiespectrales • Sensores LiDAR/ToF • HoloLens 2</td>
      </tr>
      <tr>
        <td data-es="Entornos" data-en="Environments"><strong>Entornos</strong></td>
        <td data-es="Linux • VS Code • Git • Office" data-en="Linux • VS Code • Git • Office">Linux • VS Code • Git • Office</td>
      </tr>
    </table>
  </div>
</section>

<!-- Sección: Experiencia profesional -->
<section>
  <h2 class="section-header" 
      data-es="📚 Experiencia profesional" 
      data-en="📚 Professional Experience" 
      onclick="toggleContent('experiencia')">
    📚 Experiencia profesional
  </h2>
  <img src="https://via.placeholder.com/400x200?text=Experiencia" alt="Imagen Experiencia" onclick="toggleContent('experiencia')">
  <div id="experiencia" class="content">
    <ul>
      <li data-es="🔬 Investigadora Predoctoral | INIA-CSIC (2024 - actualidad)  
          Fenotipado automatizado de cultivos con robótica y visión computacional. Diseño experimental y análisis de datos fenotípicos."
          data-en="🔬 Predoctoral Researcher | INIA-CSIC (2024 - Present)  
          Automated crop phenotyping with robotics and computer vision. Experimental design and analysis of phenotypic data.">
        🔬 <strong>Investigadora Predoctoral</strong> | INIA-CSIC (2024 - actualidad)<br>
          Fenotipado automatizado de cultivos con robótica y visión computacional. Diseño experimental y análisis de datos fenotípicos.
      </li>
      <li data-es="🧫 Técnico de Anatomía Patológica | HM Hospitales (2016)  
          Procesamiento y análisis de muestras biológicas y técnicas histológicas."
          data-en="🧫 Pathological Anatomy Technician | HM Hospitales (2016)  
          Processing and analysis of biological samples and histological techniques.">
        🧫 <strong>Técnico de Anatomía Patológica</strong> | HM Hospitales (2016)<br>
          Procesamiento y análisis de muestras biológicas y técnicas histológicas.
      </li>
      <li data-es="📞 Teleoperadora Comercial | My Assessor Total (2021)  
          Primer contacto con el mundo laboral. Aprender cómo funciona el empleo fuera del ámbito científico."
          data-en="📞 Commercial Operator | My Assessor Total (2021)  
          First contact with the working world. Learning how employment works outside the scientific field.">
        📞 <strong>Teleoperadora Comercial</strong> | My Assessor Total (2021)<br>
          Primer contacto con el mundo laboral. Aprender cómo funciona el empleo fuera del ámbito científico.
      </li>
    </ul>
  </div>
</section>

<!-- Sección: Idiomas -->
<section>
  <h2 class="section-header" 
      data-es="🌐 Idiomas" 
      data-en="🌐 Languages" 
      onclick="toggleContent('idiomas')">
    🌐 Idiomas
  </h2>
  <img src="https://via.placeholder.com/400x200?text=Idiomas" alt="Imagen Idiomas" onclick="toggleContent('idiomas')">
  <div id="idiomas" class="content">
    <ul>
      <li data-es="🇪🇸 Español: Nativo" data-en="🇪🇸 Spanish: Native">🇪🇸 Español: Nativo</li>
      <li data-es="🇬🇧 Inglés: Nivel C (APTIS - British Council)" data-en="🇬🇧 English: Level C (APTIS - British Council)">🇬🇧 Inglés: Nivel C (APTIS - British Council)</li>
      <li data-es="🇫🇷 Francés: Nivel A2 (DELF)" data-en="🇫🇷 French: Level A2 (DELF)">🇫🇷 Francés: Nivel A2 (DELF)</li>
    </ul>
  </div>
</section>

<!-- Sección: Contacto (datos) -->
<section>
  <h2 class="section-header" 
      data-es="📫 Contacto" 
      data-en="📫 Contact" 
      onclick="toggleContent('contacto')">
    📫 Contacto
  </h2>
  <img src="https://via.placeholder.com/400x200?text=Contacto" alt="Imagen Contacto" onclick="toggleContent('contacto')">
  <div id="contacto" class="content">
    <ul>
      <li data-es="✉️ Email: " data-en="✉️ Email: ">✉️ Email: <a href="mailto:andeande.ac@gmail.com">andeande.ac@gmail.com</a></li>
      <li data-es="🔗 LinkedIn: " data-en="🔗 LinkedIn: ">🔗 LinkedIn: <a href="https://www.linkedin.com/in/andreaclementeure%C3%B1a/" target="_blank">https://www.linkedin.com/in/andreaclementeure%C3%B1a/</a></li>
      <li data-es="💻 GitHub: " data-en="💻 GitHub: ">💻 GitHub: <a href="https://github.com/andyacment" target="_blank">https://github.com/andyacment</a></li>
    </ul>
  </div>
</section>

<!-- Formulario de contacto -->
<form id="contact-form">
  <h2 data-es="Formulario de Contacto" data-en="Contact Form">Formulario de Contacto</h2>
  <label for="name" data-es="Nombre" data-en="Name">Nombre</label>
  <input type="text" id="name" name="name" required>
  <label for="email" data-es="Correo electrónico" data-en="Email">Correo electrónico</label>
  <input type="email" id="email" name="email" required>
  <label for="message" data-es="Mensaje" data-en="Message">Mensaje</label>
  <textarea id="message" name="message" rows="5" required></textarea>
  <input type="submit" value="Enviar">
</form>

<footer>
  <p data-es="_&quot;La IA no es el enemigo, es la lupa que amplifica lo que la ciencia aún no alcanza.&quot; 🤖🔬🌍" 
     data-en="_&quot;AI is not the enemy; it is the magnifying glass that amplifies what science has not yet reached.&quot; 🤖🔬🌍">
    _"La IA no es el enemigo, es la lupa que amplifica lo que la ciencia aún no alcanza."_ 🤖🔬🌍
  </p>
</footer>

<script>
  function toggleContent(id) {
    var content = document.getElementById(id);
    content.style.display = content.style.display === "block" ? "none" : "block";
  }

  function toggleLanguage() {
    // Cambia el atributo lang del documento
    const lang = document.documentElement.lang === 'es' ? 'en' : 'es';
    document.documentElement.lang = lang;
    // Cambia el texto de los elementos que tienen data-es y data-en
    const elements = document.querySelectorAll('[data-es]');
    elements.forEach(el => {
      el.innerHTML = el.getAttribute('data-' + lang);
    });
    // Actualiza el texto del botón
    document.getElementById("language-toggle").innerText = lang === 'es' ? "English" : "Español";
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
