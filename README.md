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
  </style>
</head>
<body>

  <header>
    <h1>👩‍🔬 Andrea Clemente-Ureña</h1>
    <p>Bienvenid@ a mi portfolio. Aquí comparto mi trayectoria en <strong>biología</strong>, <strong>bioinformática</strong>, <strong>robótica</strong> y <strong>visión computacional 3D</strong>.</p>
    <p><strong>Investigadora predoctoral</strong> en UPM y CRF-INIA-CSIC | Proyecto: Transformación digital de la conservación y mejora vegetal</p>
  </header>

  <h2>💡 Mi primer contacto con la investigación</h2>
  <p>En 1º de Bachillerato desarrollé un proyecto sobre la <strong>síntesis de bioplásticos a partir de leche de vaca en las asignaturas de biología y técnicas experimentales en ciencias</strong> y participé en el <strong>Finde Científico</strong> realizando experimentos de química visual para divulgación.</p>
  
<div style="display: flex; gap: 20px; justify-content: center; flex-wrap: wrap;">
  <a href="https://github.com/user-attachments/assets/2507bf89-76fb-4903-b5fb-6aea3606fc46" target="_blank">
    <img src="https://github.com/user-attachments/assets/2507bf89-76fb-4903-b5fb-6aea3606fc46" alt="Imagen 1" width="300">
  </a>
  <a href="https://github.com/user-attachments/assets/fda0a450-37c9-4553-8ba1-94f0d26d670c" target="_blank">
    <img src="https://github.com/user-attachments/assets/fda0a450-37c9-4553-8ba1-94f0d26d670c" alt="Imagen 2" width="300">
  </a>
</div>

  <hr>

  <h2>🚀 Proyectos destacados</h2>

  <h3>🌱 Fenotipado de alto rendimiento</h3>
  <ul>
    <li>Integración de sensores RGB, multiespectrales y LiDAR en robots autónomos.</li>
    <li>Procesamiento de datos 3D y modelos de IA para el análisis de cultivos.</li>
  </ul>
  <img src="img/fenotipado.jpg" alt="Robot agrícola">

  <h3>🧬 Bioinformática y análisis ómico</h3>
  <p>TFM: <em>Identificación y caracterización de tRFs sobreexpresados en enfermedad de Huntington</em><br>
    📄 DOI: <a href="https://doi.org/10.13140/RG.2.2.33680.32001">10.13140/RG.2.2.33680.32001</a>
  </p>
  <img src="img/huntington_bioinfo.jpg" alt="Análisis ómico" class="center-img">

  <h3>🧪 Genética molecular y citología</h3>
  <p>TFG: <em>Caracterización estructural de genes codificantes de proteínas ribosómicas en Leishmania</em><br>
    📄 DOI: <a href="https://doi.org/10.13140/RG.2.2.10192.21767">10.13140/RG.2.2.10192.21767</a><br>
    📰 Mencionada en el <a href="https://www.cbm.uam.es/wp-content/uploads/2024/07/CBM-Scientific-Report-2021-2022.pdf">Informe Científico CBMSO-CSIC 2021–2022</a>
  </p>
  <img src="img/leishmania.jpg" alt="Leishmania" class="center-img">

  <h3>🧫 Histología e inmunohistoquímica</h3>
  <p>Proyecto sobre detección de BRCA en cáncer de mama durante el FPII.</p>
  <img src="img/histo_brca.jpg" alt="Histología BRCA">

  <h3>🥽 Tecnologías inmersivas</h3>
  <p>Colaboración con el <strong>Centro de Automática y Robótica (CAR-CSIC-UPM)</strong> en desarrollo de aplicaciones con <strong>Microsoft HoloLens 2</strong> para agricultura. (Proyecto en fase inicial)</p>

  <hr>

  <h2>🎓 Formación académica</h2>
  <ul>
    <li><strong>Doctorado en Automática y Robótica</strong><br> UPM – INIA-CSIC (2024 - actualidad)</li>
    <li><strong>Máster en Bioinformática y Bioestadística</strong><br> UOC / UB (2022 - 2024)</li>
    <li><strong>Grado en Biología</strong><br> Universidad Autónoma de Madrid (2016 - 2021)</li>
    <li><strong>Técnico Superior en Anatomía Patológica y Citología</strong><br> CESUR II (2014 - 2016)</li>
  </ul>

  <h2>🛠️ Tecnologías y herramientas</h2>
  <table>
    <tr><th>Lenguajes</th><td>Python • R • SQL • BASH • HTML/CSS</td></tr>
    <tr><th>Ciencia & Bioinfo</th><td>Bioconductor • SPSS • Galaxy • Novopath • Inferencia estadística</td></tr>
    <tr><th>IA / Visión</th><td>OpenCV • PyTorch • TensorFlow • Scikit-learn • Visión 3D</td></tr>
    <tr><th>Robótica</th><td>RGB • Multiespectrales • LiDAR/ToF • HoloLens 2</td></tr>
    <tr><th>Entornos</th><td>Linux • VS Code • Git • Office</td></tr>
  </table>

  <h2>📚 Experiencia profesional</h2>
  <ul>
    <li><strong>Investigadora Predoctoral</strong> | INIA-CSIC (2024 - actualidad)<br>
      Fenotipado automatizado de cultivos con robótica y visión computacional. Análisis de datos fenotípicos.</li>
    <li><strong>Técnico en Anatomía Patológica</strong> | HM Hospitales (2016)<br>
      Procesamiento y análisis histológico de muestras biológicas.</li>
    <li><strong>Teleoperadora Comercial</strong> | My Assessor Total (2021)<br>
      Primer empleo fuera del mundo científico. Desarrollo de habilidades interpersonales y de comunicación.</li>
  </ul>

  <h2>🌐 Idiomas</h2>
  <ul>
    <li>🇪🇸 Español: Nativo</li>
    <li>🇬🇧 Inglés: Nivel C (APTIS – British Council)</li>
    <li>🇫🇷 Francés: Nivel A2 (DELF)</li>
  </ul>

  <h2>📫 Contacto</h2>
  <ul>
    <li>✉️ Email: <a href="mailto:andeande.ac@gmail.com">andeande.ac@gmail.com</a></li>
    <li>🔗 LinkedIn: <a href="https://www.linkedin.com/in/andreaclementeure%C3%B1a/">Perfil</a></li>
    <li>💻 GitHub: <a href="https://github.com/andreaclemente96">andreaclemente96</a></li>
  </ul>

  <footer>
    <p>_"La IA no es el enemigo, es la lupa que amplifica lo que la ciencia aún no alcanza."_ 🤖🔬🌍</p
