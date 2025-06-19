<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Hotel Rosario Martín</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: #f9f9f9;
      color: #333;
    }
    header {
      background: #006494;
      color: #fff;
      text-align: center;
      padding: 1rem 0;
    }
    nav {
      background: #004d73;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
    }
    nav a {
      color: #fff;
      padding: 1rem;
      text-decoration: none;
    }
    nav a:hover {
      background: #00374f;
    }
    .container {
      max-width: 1200px;
      padding: 1rem;
      margin: auto;
    }
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px,1fr));
      gap: 10px;
      margin-bottom: 2rem;
    }
    .gallery img {
      width: 100%;
      height: auto;
      border-radius: 8px;
    }
    section {
      margin-bottom: 3rem;
    }
    h2 {
      color: #006494;
      margin-top: 0;
    }
    form {
      display: grid;
      gap: 0.5rem;
      max-width: 400px;
    }
    form input, form select, form textarea, form button {
      padding: 0.5rem;
      font-size: 1rem;
      border: 1px solid #ccc;
      border-radius: 4px;
      width: 100%;
    }
    form button {
      background: #006494;
      color: white;
      border: none;
      cursor: pointer;
    }
    form button:hover {
      background: #004d73;
    }
    .mapa {
      width: 100%;
      max-width: 600px;
      height: 350px;
      border: 0;
      margin: 1rem 0;
      border-radius: 8px;
    }
    footer {
      background: #004d73;
      color: #fff;
      text-align: center;
      padding: 1rem 0;
    }
    @media (max-width: 600px) {
      nav { flex-direction: column; }
    }
  </style>
</head>
<body>

  <header>
    <h1>Hotel Rosario Martín</h1>
    <p>Tefía, Fuerteventura – Tranquilidad y aventura en un entorno natural</p>
  </header>

  <nav>
    <a href="#inicio">Inicio</a>
    <a href="#galeria">Galería</a>
    <a href="#reservas">Reservas</a>
    <a href="#actividades">Cosas que hacer</a>
    <a href="#contacto">Contacto</a>
  </nav>

  <div class="container">

    <section id="inicio">
      <h2>Bienvenidos</h2>
      <p>Descubre nuestro acogedor hotel rural en el corazón de Fuerteventura. Ideal para relajarse, conectar con la naturaleza y vivir experiencias auténticas.</p>
    </section>

    <section id="galeria">
      <h2>Galería</h2>
      <div class="gallery">
        <img src="https://via.placeholder.com/400x300?text=Hotel+1" alt="Entrada del hotel">
        <img src="https://via.placeholder.com/400x300?text=Hotel+2" alt="Habitación doble">
        <img src="https://via.placeholder.com/400x300?text=Hotel+3" alt="Zonas comunes">
        <img src="https://via.placeholder.com/400x300?text=Hotel+4" alt="Jardín y piscina">
      </div>
    </section>

    <section id="reservas">
      <h2>Reservas</h2>
      <p>Rellena el siguiente formulario y te responderemos lo antes posible:</p>
      <form action="mailto:reservas@rosariomartinhotel.com" method="post" enctype="text/plain">
        <input type="text" name="Nombre" placeholder="Tu nombre" required>
        <input type="email" name="Email" placeholder="Tu email" required>
        <input type="tel" name="Teléfono" placeholder="Teléfono de contacto" required>
        <label>Fecha de llegada:</label>
        <input type="date" name="Llegada" required>
        <label>Fecha de salida:</label>
        <input type="date" name="Salida" required>
        <label>Habitaciones:</label>
        <select name="Habitaciones">
          <option>1</option><option>2</option><option>3</option>
        </select>
        <label>Mensaje:</label>
        <textarea name="Mensaje" rows="4" placeholder="Consultas especiales..."></textarea>
        <button type="submit">Enviar reserva</button>
      </form>
    </section>

    <section id="actividades">
      <h2>Cosas que hacer</h2>
      <ul>
        <li>Visitar el Ecomuseo La Alcogida</li>
        <li>Rutas de senderismo y bicicleta por paisajes volcánicos</li>
        <li>Excursión a Puerto del Rosario y playas cercanas</li>
        <li>Observación de estrellas en noches despejadas</li>
      </ul>
    </section>

    <section id="contacto">
      <h2>Contacto</h2>
      <ul>
        <li>Teléfono: <strong>+34 600 123 456</strong></li>
        <li>Email: <strong>info@rosariomartinhotel.com</strong></li>
        <li>Dirección: Calle Central 1, Tefía, Fuerteventura (España)</li>
      </ul>
      <iframe class="mapa" src="https://www.google.com/maps?q=28.425,-13.873&output=embed" aria-label="Mapa de ubicación"></iframe>
    </section>

  </div>

  <footer>
    <p>&copy; 2025 Hotel Rosario Martín – Todos los derechos reservados</p>
  </footer>

</body>
</html>
