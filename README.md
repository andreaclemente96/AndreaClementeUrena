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
    /* Ocultamos los títulos de sección (los h2) para que no se muestren */
    h2 { display: none; }
    header h1 {
      text-align: center;
      color: #2c3e50;
    }
    header p {
      text-align: center;
      color: #2c3e50;
    }
    img {
      border-radius: 10px;
      margin: 1rem 0;
      cursor: pointer;
      display: block;
      margin-left: auto;
      margin-right: auto;
    }
    /* Ajustamos las imágenes principales de cada sección para que sean de un tamaño adecuado */
    .section-img {
      width: 300px; /* Puedes ajustar este valor */
    }
    .content {
      display: none;
      margin-top: 10px;
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
    /* Formulario de contacto */
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
    /* Estilos para las miniaturas de los proyectos */
    .project-thumbnails {
      display: flex;
      gap: 10px;
      flex-wrap: wrap;
      justify-content: center;
      margin-top: 10px;
    }
    .thumbnail {
      width: 100px; /* Tamaño similar a un post-it */
      border: 1px solid #ccc;
      border-radius: 5px;
      overflow: hidden;
    }
    .thumbnail img {
      width: 100%;
      display: block;
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
  <!-- Solo imagen con tooltip; al pasar el ratón se verá el título -->
  <img class="section-img" src="https://via.placeholder.com/300?text=Bienvenida" alt="Bienvenida" title="¡Bienvenid@ a mi portfolio!">
  <div class="content" style="display: block;"> 
    <!-- Contenido de bienvenida (si lo deseas mostrar al hacer clic, aquí lo dejamos visible por defecto) -->
    <p>
      <span class="lang-es">Este espacio reúne mi trayectoria en <strong>biología</strong>, <strong>bioinformática</strong>, <strong>robótica</strong> y <strong>visión computacional 3D</strong>. Actualmente desarrollo herramientas avanzadas para el <strong>fenotipado de cultivos</strong> y la <strong>caracterización de estructuras vegetales</strong>, aplicando aprendizaje automático y análisis de datos.</span>
      <span class="lang-en">This space brings together my journey in <strong>biology</strong>, <strong>bioinformatics</strong>, <strong>robotics</strong> and <strong>3D computer vision</strong>. I currently develop advanced tools for <strong>crop phenotyping</strong> and <strong>plant structure characterization</strong> using machine learning and data analysis.</span>
    </p>
    <p>
      <span class="lang-es">📍 Investigadora predoctoral en la Universidad Politécnica de Madrid (UPM) y el Centro de Recursos Fitogenéticos (CRF-INIA-CSIC), dentro del proyecto <strong>Transformación digital de las actividades de conservación y mejora vegetal</strong>.</span>
      <span class="lang-en">📍 Predoctoral researcher at the Polytechnic University of Madrid (UPM) and the Fitogenetic Resources Center (CRF-INIA-CSIC), in the project <strong>Digital Transformation of Plant Conservation and Improvement</strong>.</span>
    </p>
  </div>
</section>

<!-- Sección: Mi primer contacto con la investigación -->
<section id="primer-contacto-section">
  <!-- Solo imagen con tooltip; la imagen es visible -->
  <img class="section-img" src="https://img.freepik.com/foto-gratis/lapices-compuestos-pizarra_1313812.jpg" alt="Mi primer contacto con la investigación" title="💡 Mi primer contacto con la investigación" onclick="toggleContent('primer_contacto')">
  <div id="primer_contacto" class="content">
    <p>
      <span class="lang-es">Mi primer contacto con la investigación fue en 1º de Bachillerato, cuando desarrollé un proyecto sobre la <em>síntesis de bioplásticos a partir de la leche de vaca</em> en las asignaturas de Biología y Técnicas Experimentales en Ciencias. Ese mismo año participé en el <strong>Finde Científico</strong>, formando parte de un equipo que realizaba experimentos de química visual para la divulgación científica.</span>
      <span class="lang-en">My first encounter with research was in the first year of high school when I developed a project on the <em>synthesis of bioplastics from cow's milk</em> in Biology and Experimental Techniques classes. That same year, I participated in Finde Científico, as part of a team performing visual chemistry experiments to bring science closer to the public.</span>
    </p>
    <div style="display: flex; justify-content: center; gap: 20px;">
      <img src="https://github.com/user-attachments/assets/2507bf89-76fb-4903-b5fb-6aea3606fc46" alt="Síntesis de bioplásticos" width="300" title="Síntesis de bioplásticos">
      <img src="https://github.com/user-attachments/assets/fda0a450-37c9-4553-8ba1-94f0d26d670c" alt="Finde Científico" width="300" title="Finde Científico">
    </div>
  </div>
</section>

<!-- Sección: Proyectos destacados -->
<section id="proyectos-section">
  <!-- Solo imagen principal; al hacer clic se despliegan las miniaturas -->
  <img class="section-img" src="https://via.placeholder.com/300?text=Proyectos" alt="Proyectos Destacados" title="🚀 Proyectos destacados" onclick="toggleContent('proyectos-thumbnails')">
  <div id="proyectos-thumbnails" class="content">
    <!-- Aquí se muestran solo las miniaturas (sin texto) -->
    <div class="project-thumbnails">
      <div class="thumbnail" title="Fenotipado de alto rendimiento" onclick="toggleContent('proyecto1')">
        <img src="https://via.placeholder.com/100?text=Img+1" alt="Miniatura 1">
      </div>
      <div class="thumbnail" title="Bioinformática y análisis ómico" onclick="toggleContent('proyecto2')">
        <img src="https://via.placeholder.com/100?text=Img+2" alt="Miniatura 2">
      </div>
      <div class="thumbnail" title="Genética molecular y citología" onclick="toggleContent('proyecto3')">
        <img src="https://via.placeholder.com/100?text=Img+3" alt="Miniatura 3">
      </div>
      <div class="thumbnail" title="Histología e inmunohistoquímica" onclick="toggleContent('proyecto4')">
        <img src="https://via.placeholder.com/100?text=Img+4" alt="Miniatura 4">
      </div>
      <div class="thumbnail" title="Exploración con tecnologías inmersivas" onclick="toggleContent('proyecto5')">
        <img src="https://via.placeholder.com/100?text=Img+5" alt="Miniatura 5">
      </div>
    </div>
    <!-- Detalles de cada proyecto (se muestran al hacer clic en la miniatura correspondiente) -->
    <div id="proyecto1" class="content">
      <!-- Aquí colocas los detalles de "Fenotipado de alto rendimiento" -->
      <p>
        <span class="lang-es">Detalles del proyecto de fenotipado de alto rendimiento...</span>
        <span class="lang-en">Details of the high-performance phenotyping project...</span>
      </p>
    </div>
    <div id="proyecto2" class="content">
      <p>
        <span class="lang-es">Detalles del proyecto de bioinformática y análisis ómico...</span>
        <span class="lang-en">Details of the bioinformatics and omics analysis project...</span>
      </p>
    </div>
    <div id="proyecto3" class="content">
      <p>
        <span class="lang-es">Detalles del proyecto de genética molecular y citología...</span>
        <span class="lang-en">Details of the molecular genetics and cytology project...</span>
      </p>
    </div>
    <div id="proyecto4" class="content">
      <p>
        <span class="lang-es">Detalles del proyecto de histología e inmunohistoquímica...</span>
        <span class="lang-en">Details of the histology and immunohistochemistry project...</span>
      </p>
    </div>
    <div id="proyecto5" class="content">
      <p>
        <span class="lang-es">Detalles del proyecto de exploración con tecnologías inmersivas...</span>
        <span class="lang-en">Details of the exploration with immersive technologies project...</span>
      </p>
    </div>
  </div>
</section>

<!-- Sección: Formación académica -->
<section id="formacion-section">
  <img class="section-img" src="https://via.placeholder.com/300?text=Formaci%C3%B3n" alt="Formación Académica" title="🎓 Formación académica" onclick="toggleContent('formacion')">
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
<section id="tecnologias-section">
  <img class="section-img" src="https://via.placeholder.com/300?text=Tecnolog%C3%ADas" alt="Tecnologías y Herramientas" title="🛠️ Tecnologías y herramientas" onclick="toggleContent('tecnologias')">
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
<section id="experiencia-section">
  <img class="section-img" src="https://via.placeholder.com/300?text=Experiencia" alt="Experiencia Profesional" title="📚 Experiencia profesional" onclick="toggleContent('experiencia')">
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
<section id="idiomas-section">
  <img class="section-img" src="https://via.placeholder.com/300?text=Idiomas" alt="Idiomas" title="🌐 Idiomas" onclick="toggleContent('idiomas')">
  <div id="idiomas" class="content">
    <ul>
      <li><span class="lang-es">🇪🇸 Español: Nativo</span><span class="lang-en">🇪🇸 Spanish: Native</span></li>
      <li><span class="lang-es">🇬🇧 Inglés: Nivel C (APTIS - British Council)</span><span class="lang-en">🇬🇧 English: Level C (APTIS - British Council)</span></li>
      <li><span class="lang-es">🇫🇷 Francés: Nivel A2 (DELF)</span><span class="lang-en">🇫🇷 French: Level A2 (DELF)</span></li>
    </ul>
  </div>
</section>

<!-- Sección: Contacto (datos) -->
<section id="contacto-section">
  <img class="section-img" src="https://via.placeholder.com/300?text=Contacto" alt="Contacto" title="📫 Contacto" onclick="toggleContent('contacto')">
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
    alert("Formulario enviado. Gracias por tu mensaje.");
    this.reset();
  });
</script>

</body>
</html>

