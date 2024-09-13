
  <title>Perfil de Percy</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f4f4f4;
      color: #333;
      margin: 0;
      padding: 0;
    }

    header {
      background-color: #333;
      color: #fff;
      padding: 10px 0;
      text-align: center;
    }

    .container {
      width: 80%;
      margin: auto;
      overflow: hidden;
    }

    .section {
      padding: 20px 0;
    }

    h2 {
      text-align: center;
      color: #333;
    }

    .projects, .skills {
      display: flex;
      justify-content: space-around;
      flex-wrap: wrap;
    }

    .project, .skill {
      background-color: #fff;
      border: 1px solid #ddd;
      border-radius: 8px;
      margin: 10px;
      width: 30%;
      padding: 20px;
      text-align: center;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }

    .project img {
      width: 100%;
      height: auto;
      border-radius: 8px;
    }

    .project h3, .skill h3 {
      margin-top: 15px;
    }

    .skill img {
      width: 50px;
      height: 50px;
    }

    footer {
      background-color: #333;
      color: #fff;
      padding: 10px 0;
      text-align: center;
    }
  </style>
</head>
<body>

  <header>
    <h1>Perfil de Percy</h1>
    <p>Estudiante de programación | JavaScript, Java, C# y Diseño Gráfico</p>
  </header>

  <div class="container">
    <!-- Sección de proyectos -->
    <section class="section">
      <h2>Mis Proyectos</h2>
      <div class="projects">
        <div class="project">
          <img src="ruta_de_la_imagen_del_proyecto_1.jpg" alt="Proyecto 1">
          <h3>Proyecto Empresa X</h3>
          <p>Página web para gestión de clientes.</p>
        </div>
        <div class="project">
          <img src="ruta_de_la_imagen_del_proyecto_2.jpg" alt="Proyecto 2">
          <h3>Proyecto Empresa Y</h3>
          <p>Tienda online para venta de productos.</p>
        </div>
        <div class="project">
          <img src="ruta_de_la_imagen_del_proyecto_3.jpg" alt="Proyecto 3">
          <h3>Proyecto Empresa Z</h3>
          <p>Plataforma interna de comunicación empresarial.</p>
        </div>
      </div>
    </section>
    <section class="section">
      <h2>Lenguajes y Habilidades</h2>
      <div class="skills">
        <div class="skill">
          <img src="ruta_de_la_imagen_js.png" alt="JavaScript">
          <h3>JavaScript</h3>
        </div>
        <div class="skill">
          <img src="ruta_de_la_imagen_java.png" alt="Java">
          <h3>Java</h3>
        </div>
        <div class="skill">
          <img src="ruta_de_la_imagen_csharp.png" alt="C#">
          <h3>C#</h3>
        </div>
        <div class="skill">
          <img src="ruta_de_la_imagen_design.png" alt="Diseño Gráfico">
          <h3>Diseño Gráfico</h3>
        </div>
      </div>
    </section>
  </div>

  <footer>
    <p>&copy; 2024 Percy - Todos los derechos reservados</p>
  </footer>

  <script>
    // Puedes agregar aquí alguna interacción con JavaScript
  </script>

</body>
</html>
