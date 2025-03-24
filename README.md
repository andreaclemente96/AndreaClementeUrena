<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio Andrea Clemente-Ureña</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
        }
        header {
            background-color: #4CAF50;
            color: white;
            padding: 15px;
            text-align: center;
        }
        section {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-around;
            padding: 20px;
        }
        .section {
            width: 100%;
            margin: 10px;
            padding: 20px;
            background-color: white;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
        }
        .section img {
            width: 100%;
            height: auto;
            border-radius: 8px;
        }
        .section h2 {
            font-size: 24px;
            margin-top: 10px;
        }
        .section p {
            font-size: 16px;
            color: #333;
        }
        .collapse {
            display: none;
            padding-top: 10px;
            font-size: 16px;
            color: #555;
        }
        .section-button {
            padding: 10px;
            background-color: #4CAF50;
            color: white;
            border: none;
            width: 100%;
            cursor: pointer;
            text-align: center;
            border-radius: 8px;
        }
        .section-button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <header>
        <h1>👩‍🔬 Andrea Clemente-Ureña</h1>
        <p>¡Bienvenid@ a mi portfolio! Este espacio reúne mi trayectoria en biología, bioinformática, robótica y visión computacional 3D. Actualmente desarrollo herramientas avanzadas para el fenotipado de cultivos y la caracterización de estructuras vegetales, aplicando aprendizaje automático y análisis de datos.</p>
        <p>📍 Investigadora predoctoral en la Universidad Politécnica de Madrid (UPM) y el Centro de Recursos Fitogenéticos (CRF-INIA-CSIC), dentro del proyecto **Transformación digital de las actividades de conservación y mejora vegetal**.</p>
    </header>

    <section>
        <div class="section">
            <button class="section-button" onclick="toggleSection('section1')">💡 Mi primer contacto con la investigación</button>
            <div id="section1" class="collapse">
                <p>Mi primer contacto con la investigación fue en 1º de Bachillerato, cuando desarrollé un proyecto sobre la síntesis de bioplásticos a partir de la leche de vaca en las asignaturas de Biología y Técnicas Experimentales en Ciencias. Ese mismo año participé en el Finde Científico, formando parte de un equipo que realizaba experimentos de química visual (cambio de color gracias a las reacciones) para la divulgación científica, diseñados para acercar la ciencia a estudiantes, niños y familias en general.</p>
            </div>
        </div>

        <div class="section">
            <button class="section-button" onclick="toggleSection('section2')">🚀 Proyectos destacados</button>
            <div id="section2" class="collapse">
                <h2>🌱 Fenotipado de alto rendimiento</h2>
                <p>Integración de sensores RGB, multiespectrales y LiDAR en robots autónomos. Procesamiento de datos 3D y modelos de IA para el análisis de cultivos.</p>
                <img src="image1.jpg" alt="Fenotipado de alto rendimiento">
                
                <h2>🧬 Bioinformática y análisis ómico</h2>
                <p>TFM: Identificación y caracterización de tRFs sobreexpresados en enfermedad de Huntington. DOI: 10.13140/RG.2.2.33680.32001</p>
                <img src="image2.jpg" alt="Bioinformática y análisis ómico">
                
                <h2>🧪 Genética molecular y citología</h2>
                <p>TFG: Caracterización estructural de genes codificantes de proteínas ribosómicas en Leishmania. DOI: 10.13140/RG.2.2.10192.21767</p>
                <img src="image3.jpg" alt="Genética molecular y citología">
                
                <h2>🧫 Histología e inmunohistoquímica</h2>
                <p>Proyecto sobre detección inmunohistoquímica de BRCA en cáncer de mama durante el FPII.</p>
                <img src="image4.jpg" alt="Histología e inmunohistoquímica">
            </div>
        </div>

        <div class="section">
            <button class="section-button" onclick="toggleSection('section3')">🥽 Exploración con tecnologías inmersivas</button>
            <div id="section3" class="collapse">
                <p>Actualmente colaboro con el Centro de Automática y Robótica (CAR-CSIC-UPM), donde estoy comenzando a desarrollar soluciones con Microsoft HoloLens2, centradas en aplicaciones innovadoras dentro del entorno agrícola. (Proyecto en fase inicial)</p>
                <img src="hololens.jpg" alt="Exploración con tecnologías inmersivas">
            </div>
        </div>

        <div class="section">
            <button class="section-button" onclick="toggleSection('section4')">🎓 Formación académica</button>
            <div id="section4" class="collapse">
                <p><strong>📘 Doctorado en Automática y Robótica</strong><br>Universidad Politécnica de Madrid – INIA-CSIC (2024 - actualidad)</p>
                <p><strong>📊 Máster en Bioinformática y Bioestadística</strong><br>Universitat Oberta de Catalunya / Universitat de Barcelona (2022 - 2024)</p>
                <p><strong>🧬 Grado en Biología</strong><br>Universidad Autónoma de Madrid (2016 - 2021)</p>
                <p><strong>🔬 Técnico Superior en Anatomía Patológica y Citología</strong><br>CESUR II (2014 - 2016)</p>
            </div>
        </div>

        <div class="section">
            <button class="section-button" onclick="toggleSection('section5')">🛠️ Tecnologías y herramientas</button>
            <div id="section5" class="collapse">
                <ul>
                    <li>Lenguajes: Python, R, SQL, BASH, HTML/CSS</li>
                    <li>Ciencia & Bioinfo: Bioconductor, SPSS, Galaxy, Novopath, Inferencia estadística</li>
                    <li>IA / Visión: OpenCV, PyTorch, TensorFlow, Scikit-learn, Visión 3D</li>
                    <li>Robótica: Sensores RGB, Sensores Multiespectrales, Sensores LiDAR/ToF, HoloLens 2</li>
                    <li>Entornos: Linux, VS Code, Git, Office</li>
                </ul>
            </div>
        </div>

        <div class="section">
            <button class="section-button" onclick="toggleSection('section6')">📚 Experiencia profesional</button>
            <div id="section6" class="collapse">
                <p><strong>🔬 Investigadora Predoctoral:</strong> INIA-CSIC (2024 - actualidad)</p>
                <p><strong>🧫 Técnico de Anatomía Patológica:</strong> HM Hospitales (2016)</p>
                <p><strong>📞 Teleoperadora Comercial:</strong> My Assessor Total (2021)</p>
            </div>
        </div>

        <div class="section">
            <button class="section-button" onclick="toggleSection('section7')">🌐 Idiomas</button>
            <div id="section7" class="collapse">
                <p>🇪🇸 Español: Nativo</p>
                <p>🇬🇧 Inglés: Nivel C (APTIS - British Council)</p>
                <p>🇫🇷 Francés: Nivel A2 (DELF)</p>
            </div>
        </div>

        <div class="section">
            <button class="section-button" onclick="toggleSection('section8')">📫 Contacto</button>
            <div id="section8" class="collapse">
                <p><strong>Email:</strong> andeande.ac@gmail.com</p>
                <p><strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/andreaclementeure%C3%B1a/">Andrea Clemente Ureña</a></p>
                <p><strong>GitHub:</strong> <a href="https://github.com/andreaclemente96">GitHub</a></p>
            </div>
        </div>
    </section>

    <script>
        function toggleSection(sectionId) {
            const section = document.getElementById(sectionId);
            section.style.display = section.style.display === "block" ? "none" : "block";
        }
    </script>
</body>
</html>

---
##  _"La IA no es el enemigo, es la lupa que amplifica lo que la ciencia aún no alcanza. "_ 🤖🔬🌍
Andrea Clemente Ureña
