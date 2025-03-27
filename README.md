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
  <h1 data-es="👩‍🔬 Andrea Clemente-Ureña" data-en="👩‍🔬 Andrea Clemente-Ureña">

</body>
</html>
