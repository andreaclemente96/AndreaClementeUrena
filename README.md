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
  </style>
</head>
<body>

  <header>
    <h1>👩‍🔬 Andrea Clemente-Ureña</h1>
    <p>Bienvenid@ a mi portfolio. Aquí comparto mi trayectoria en <strong>biología</strong>, <strong>bioinformática</strong>, <strong>robótica</strong> y <strong>visión computacional 3D</strong>.</p>
    <p><strong>Investigadora predoctoral</strong> en UPM y CRF-INIA-CSIC | Proyecto: Transformación digital de la conservación y mejora vegetal</p>
  </header>

  <section>
    <h2 class="section-header" onclick="toggleContent('intro')">¡Bienvenid@ a mi portfolio!</h2>
    <div id="intro" class="content">
      <p>Este espacio reúne mi trayectoria en <strong>biología</strong>, <strong>bioinformática</strong>, <strong>robótica</strong> y <strong>visión computacional 3D</strong>. Actualmente desarrollo herramientas avanzadas para el <strong>fenotipado de cultivos</strong> y la <strong>caracterización de estructuras vegetales</strong>, aplicando aprendizaje automático y análisis de datos.</p>
      <p>📍 Investigadora predoctoral en la Universidad Politécnica de Madrid (UPM) y el Centro de Recursos Fitogenéticos (CRF-INIA-CSIC), dentro del proyecto <strong>Transformación digital de las actividades de conservación y mejora vegetal</strong>.</p>
    </div>
  </section>

  <section>
    <h2 class="section-header" onclick="toggleContent('primer_contacto')">💡 Mi primer contacto con la investigación</h2>
    <div id="primer_contacto" class="content">
      <p>Mi primer contacto con la investigación fue en 1º de Bachillerato, cuando desarrollé un proyecto sobre la <strong>síntesis de bioplásticos a partir de la leche de vaca</strong> en las asignaturas de Biología y Técnicas Experimentales en Ciencias. Ese mismo año participé en el <strong>Finde Científico</strong>, formando parte de un equipo que realizaba experimentos de química visual (cambio de color gracias a las reacciones) para la divulgación científica, diseñados para acercar la ciencia a estudiantes, niños y familias en general.</p>
      <div style="display: flex; justify-content: center; gap: 20px;">
        <img src="https://github.com/user-attachments/assets/2507bf89-76fb-4903-b5fb-6aea3606fc46" alt="Síntesis de bioplásticos a partir de la leche de vaca" width="300">
        <img src="https://github.com/user-attachments/assets/fda0a450-37c9-4553-8ba1-94f0d26d670c" alt="Finde Científico: Experimentos de química visual" width="300">
      </div>
    </div>
  </section>

  <section>
    <h2 class="section-header" onclick="toggleContent('proyectos')">🚀 Proyectos destacados</h2>
    <div id="proyectos" class="content">
      <ul>
        <li><strong>Fenotipado de alto rendimiento</strong>
          <ul>
            <li>Integración de sensores RGB, multiespectrales y LiDAR en robots autónomos.</li>
            <li>Procesamiento de datos 3D y modelos de IA para el análisis de cultivos.</li>
          </ul>
          <p align="center">
            <img src="https://github.com/user-attachments/assets/9905699f-ddda-4b6a-970a-08e2fbd359aa" alt="Fenotipado de alto rendimiento" width="400">
          </p>
        </li>

        <li><strong>Bioinformática y análisis ómico</strong>
          <ul>
            <li>TFM: *Identificación y caracterización de tRFs sobreexpresados en enfermedad de Huntington*.</li>
            <li>📄 DOI: <a href="https://doi.org/10.13140/RG.2.2.33680.32001" target="_blank">10.13140/RG.2.2.33680.32001</a></li>
          </ul>
          <p align="center">
            <img src="https://github.com/user-attachments/assets/8dfa2628-f892-4078-bde3-3915150bed34" alt="Bioinformática y análisis ómico" width="400">
          </p>
        </li>

        <li><strong>Genética molecular y citología</strong>
          <ul>
            <li>TFG: *Caracterización estructural de genes codificantes de proteínas ribosómicas en Leishmania*.</li>
            <li>📄 DOI: <a href="https://doi.org/10.13140/RG.2.2.10192.21767" target="_blank">10.13140/RG.2.2.10192.21767</a></li>
            <li>📰 Participación mencionada en el <a href="https://www.cbm.uam.es/wp-content/uploads/2024/07/CBM-Scientific-Report-2021-2022.pdf" target="_blank">Informe Científico del CBMSO-CSIC 2021–2022</a></li>
          </ul>
          <p align="center">
            <img src="https://github.com/user-attachments/assets/b740f460-1160-4a35-90c6-b3b2e5861f23" alt="Genética molecular y citología" width="400">
          </p>
        </li>

        <li><strong>Histología e inmunohistoquímica</strong>
          <ul>
            <li>Proyecto sobre detección inmunohistoquímica de BRCA en cáncer de mama durante el FPII.</li>
          </ul>
          <p align="center">
            <img src="https://github.com/user-attachments/assets/73e74b49-a323-40f3-b055-1f3bfaf9750c" alt="Histología e inmunohistoquímica" width="400">
          </p>
        </li>

        <li><strong>Exploración con tecnologías inmersivas</strong>
          <ul>
            <li>Colaboración con el <strong>Centro de Automática y Robótica (CAR-CSIC-UPM)</strong> para desarrollar soluciones con <strong>Microsoft HoloLens2</strong> en aplicaciones agrícolas. *(Proyecto en fase inicial)*</li>
          </ul>
        </li>
      </ul>
    </div>
  </section>
<section>
  <h2>🎓 Formación académica</h2>
  <ul>
    <li>📘 **Doctorado en Automática y Robótica** (2024 - actualidad) - Universidad Politécnica de Madrid – INIA-CSIC</li>
    <li>📊 **Máster en Bioinformática y Bioestadística** (2022 - 2024) - Universitat Oberta de Catalunya / Universitat de Barcelona</li>
    <li>🧬 **Grado en Biología** (2016 - 2021) - Universidad Autónoma de Madrid</li>
    <li>🔬 **Técnico Superior en Anatomía Patológica y Citología** (2014 - 2016) - CESUR II</li>
  </ul>
</section>

<section>
  <h2>🛠️ Tecnologías y herramientas</h2>
  <table>
    <tr>
      <td><strong>Lenguajes</strong></td>
      <td>Python • R • SQL • BASH • HTML/CSS</td>
    </tr>
    <tr>
      <td><strong>Ciencia & Bioinfo</strong></td>
      <td>Bioconductor • SPSS • Galaxy • Novopath • Inferencia estadística</td>
    </tr>
    <tr>
      <td><strong>IA / Visión</strong></td>
      <td>OpenCV • PyTorch • TensorFlow • Scikit-learn • Visión 3D</td>
    </tr>
    <tr>
      <td><strong>Robótica</strong></td>
      <td>Sensores RGB • Sensores Multiespectrales • Sensores LiDAR/ToF • HoloLens 2</td>
    </tr>
    <tr>
      <td><strong>Entornos</strong></td>
      <td>Linux • VS Code • Git • Office</td>
    </tr>
  </table>
</section>

<section>
  <h2>📚 Experiencia profesional</h2>
  <ul>
    <li>🔬 **Investigadora Predoctoral** | INIA-CSIC (2024 - actualidad)  
      Fenotipado automatizado de cultivos con robótica y visión computacional. Diseño experimental y análisis de datos fenotípicos.</li>
    <li>🧫 **Técnico de Anatomía Patológica** | HM Hospitales (2016)  
      Procesamiento y análisis de muestras biológicas y técnicas histológicas.</li>
    <li>📞 **Teleoperadora Comercial** | My Assessor Total (2021)  
      Primer contacto con el mundo laboral. Aprender como funciona el empleo fuera del ámbito científico.</li>
  </ul>
</section>

<section>
  <h2>🌐 Idiomas</h2>
  <ul>
    <li>🇪🇸 Español: Nativo</li>
    <li>🇬🇧 Inglés: Nivel C (APTIS - British Council)</li>
    <li>🇫🇷 Francés: Nivel A2 (DELF)</li>
  </ul>
</section>

<section>
  <h2>📫 Contacto</h2>
  <ul>
    <li>✉️ Email: <a href="mailto:andeande.ac@gmail.com">andeande.ac@gmail.com</a></li>
    <li>🔗 LinkedIn: <a href="https://www.linkedin.com/in/andreaclementeure%C3%B1a/" target="_blank">https://www.linkedin.com/in/andreaclementeure%C3%B1a/</a></li>
    <li>💻 GitHub: <a href="https://github.com/andyacment" target="_blank">https://github.com/andyacment</a></li>
  </ul>
</section>
  <footer>
    <p>_"La IA no es el enemigo, es la lupa que amplifica lo que la ciencia aún no alcanza."_ 🤖🔬🌍</p>
  </footer>

  <script>
    function toggleContent(id) {
      var content = document.getElementById(id);
      content.style.display = content.style.display === "block" ? "none" : "block";
    }
  </script>
  
</body>
</html>
