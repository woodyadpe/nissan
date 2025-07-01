
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Asesoría Nissan Expert</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css" crossorigin="anonymous" referrerpolicy="no-referrer" />
  <style>
    * {
      box-sizing: border-box;
    }

    .circle-title {
      width: 200px;
      height: 200px;
      border-radius: 50%;
      background-color: white;
      color: #cc0000;
      display: flex;
      align-items: center;
      justify-content: center;
      margin: 0 auto 20px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    }

    .circle-title h1 {
      font-size: 20px;
      text-align: center;
      margin: 0;
      padding: 10px;
    }

    @media (max-width: 480px) {
      .circle-title {
        width: 140px;
        height: 140px;
      }

      .circle-title h1 {
        font-size: 14px;
      }
    }

    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      margin: 0;
      background-color: #f8f8f8;
      color: #333;
    }

    header {
      background-color: #cc0000;
      color: white;
      text-align: center;
      padding: 40px 20px;
    }

    nav {
      background-color: #222;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
    }

    nav a {
      color: white;
      text-decoration: none;
      padding: 15px 25px;
      display: inline-block;
      transition: background 0.3s;
    }

    nav a:hover {
      background-color: #cc0000;
    }

    section {
      padding: 60px 20px;
      max-width: 1000px;
      margin: 30px auto;
      background-color: white;
      border-radius: 10px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }

    section h2 {
      color: #cc0000;
      margin-bottom: 20px;
    }

    section h3 {
      margin-top: 30px;
      color: #444;
    }

    .servicio {
      margin-bottom: 20px;
    }

    footer {
      background-color: #333;
      color: white;
      text-align: center;
      padding: 25px 0;
    }

    ul {
      padding-left: 20px;
    }

    #formulario input,
    #formulario textarea {
      width: 100%;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 6px;
      margin-bottom: 15px;
      font-size: 16px;
    }

    #formulario button {
      background-color: #25D366;
      color: white;
      border: none;
      padding: 12px 25px;
      border-radius: 6px;
      cursor: pointer;
      font-size: 16px;
      transition: background 0.3s;
    }

    #formulario button:hover {
      background-color: #1ebe5d;
    }

    #mensajeConfirmacion {
      color: green;
      margin-top: 15px;
      font-weight: bold;
      display: none;
    }

    @media (max-width: 768px) {
      nav a {
        padding: 12px 16px;
        font-size: 14px;
      }

      header h1 {
        font-size: 24px;
      }

      section {
        padding: 40px 15px;
      }
    }
  </style>
</head>
<body>
  <header>
    <div class="circle-title">
      <h1>Asesoría Nissan Expert</h1>
    </div>
    <p>Tu guía confiable para elegir, mantener y disfrutar tu Nissan</p>
  </header>

  <nav>
    <a href="#servicios">Servicios</a>
    <a href="#nosotros">Nosotros</a>
    <a href="#contacto">Contacto</a>
    <a href="#formulario">Formulario</a>
  </nav>

  <section id="servicios">
    <h2>Servicios</h2>
    <div class="servicio">
      <h3>Compra Inteligente</h3>
      <p>Asesoría completa para elegir el Nissan perfecto según tu estilo de vida, presupuesto y uso previsto.</p>
    </div>
    <div class="servicio">
      <h3>Prueba de Manejo</h3>
      <p>Te brindamos la experiencia de probar el carro de tus sueños.</p>
    </div>
    <div class="servicio">
      <h3>Mantenimiento Personalizado</h3>
      <p>Te entregamos un plan de mantenimiento adaptado al modelo de tu Nissan para que dure más y rinda mejor.</p>
    </div>
  </section>

  <section id="nosotros">
    <h2>¿Quiénes Somos?</h2>
    <p>Somos un emprendimiento apasionado por los autos Nissan...</p>
    <h3>Misión</h3>
    <p>Brindar asesoría personalizada, confiable y experta...</p>
    <h3>Visión</h3>
    <p>Ser la asesoría automotriz especializada en Nissan más reconocida...</p>
    <h3>Objetivos</h3>
    <ul>
      <li>Guiar al cliente en la elección del vehículo Nissan ideal.</li>
      <li>Ofrecer diagnósticos técnicos previos a la compra.</li>
      <li>Construir una relación transparente y profesional.</li>
    </ul>
  </section>

  <section id="contacto">
    <h2>Contacto</h2>
    <p><strong>Correo:</strong> claumira1@yahoo.com</p>
    <p><strong>Teléfono:</strong> +52 229 410 1145</p>
    <p><strong>Ubicación:</strong> Veracruz, Ver.</p>
  </section>

  <section id="formulario">
    <h2>Formulario de Contacto</h2>
    <form id="whatsappForm">
      <label for="nombre">Nombre:</label><br>
      <input type="text" id="nombre" name="nombre" required><br>

      <label for="correo">Correo electrónico:</label><br>
      <input type="email" id="correo" name="correo" required><br>

      <label for="mensaje">Mensaje:</label><br>
      <textarea id="mensaje" name="mensaje" rows="5" required></textarea><br>

      <button type="submit"><i class="fab fa-whatsapp"></i> Enviar por WhatsApp</button>
      <p id="mensajeConfirmacion">Recibimos tu mensaje, en un momento te atendemos.</p>
    </form>
  </section>

  <script>
    document.getElementById("whatsappForm").addEventListener("submit", function(event) {
      event.preventDefault();
      const nombre = document.getElementById("nombre").value.trim();
      const correo = document.getElementById("correo").value.trim();
      const mensaje = document.getElementById("mensaje").value.trim();
      const texto = Hola, soy ${nombre}. Mi correo es ${correo}. Quisiera decir: ${mensaje};
      const numero = "527298574364";
      const url = https://wa.me/${numero}?text=${encodeURIComponent(texto)};
      window.open(url, "_blank");
      document.getElementById("mensajeConfirmacion").style.display = "block";
    });
  </script>
</body>
</html>
