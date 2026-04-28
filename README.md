<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ElJefeKingg | Prioridad Nacional</title>

  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #050505;
      color: white;
      scroll-behavior: smooth;
    }

    header {
      background: linear-gradient(120deg, black, #8b0000);
      padding: 100px 20px;
      text-align: center;
      position: relative;
      overflow: hidden;
    }

    header::before {
      content: "";
      background: url('https://via.placeholder.com/1200x800') center/cover;
      opacity: 0.25;
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      z-index: 0;
    }

    header h1, header p, .cta {
      position: relative;
      z-index: 1;
    }

    header h1 {
      font-size: 60px;
      margin: 0;
      letter-spacing: 4px;
    }

    header p {
      font-size: 24px;
      color: gold;
      margin-top: 10px;
    }

    .cta a {
      background: gold;
      color: black;
      padding: 14px 28px;
      margin: 10px;
      display: inline-block;
      text-decoration: none;
      font-weight: bold;
      border-radius: 6px;
      transition: 0.3s;
    }

    .cta a:hover {
      background: red;
      color: white;
      transform: scale(1.05);
    }

    .contador {
      margin-top: 20px;
      font-size: 20px;
      color: gold;
    }

    section {
      padding: 80px 20px;
      max-width: 1000px;
      margin: auto;
    }

    .bloque {
      background: #111;
      padding: 30px;
      margin-bottom: 30px;
      border-left: 6px solid red;
      transition: 0.4s;
      transform: translateY(40px);
      opacity: 0;
    }

    .bloque.visible {
      transform: translateY(0);
      opacity: 1;
    }

    .noticias .bloque {
      border-left: 6px solid gold;
    }

    footer {
      text-align: center;
      padding: 30px;
      background: black;
      font-size: 14px;
      color: gray;
    }
  </style>
</head>

<body>

<header>
  <h1>@eljefekingg</h1>
  <p>PRIORIDAD NACIONAL</p>

  <div class="cta">
    <a href="https://www.tiktok.com/@eljefekingg" target="_blank">Ver TikTok</a>
    <a href="#videos">Ver Vídeos</a>
  </div>

  <div class="contador">
    +125.000 seguidores | +3M visualizaciones
  </div>
</header>

<section>
  <div class="bloque">
    <h2>Mensaje</h2>
    <p>
      Contenido político directo, sin filtros. Defensa de España y mensajes diseñados para despertar conciencia.
    </p>
  </div>

  <div class="bloque">
    <h2>Movimiento</h2>
    <p>
      Esto no es solo contenido. Es una comunidad en crecimiento con una idea clara: PRIORIDAD NACIONAL.
    </p>
  </div>
</section>

<section class="noticias">
  <h2>Noticias / Mensajes virales</h2>

  <div class="bloque">
    <h3>Impacto en redes</h3>
    <p>Los vídeos de @eljefekingg superan miles de visualizaciones generando debate real.</p>
  </div>

  <div class="bloque">
    <h3>Crecimiento constante</h3>
    <p>La comunidad sigue aumentando cada día con más apoyo y difusión.</p>
  </div>
</section>

<section id="videos">
  <h2>Últimos Vídeos</h2>

  <blockquote class="tiktok-embed" cite="https://www.tiktok.com/@eljefekingg" data-unique-id="eljefekingg" style="max-width: 605px;min-width: 325px;">
    <section></section>
  </blockquote>
</section>

<script async src="https://www.tiktok.com/embed.js"></script>

<script>
  const bloques = document.querySelectorAll('.bloque');

  window.addEventListener('scroll', () => {
    bloques.forEach(b => {
      const top = b.getBoundingClientRect().top;
      if (top < window.innerHeight - 100) {
        b.classList.add('visible');
      }
    });
  });
</script>

<footer>
  © 2026 ElJefeKingg | Web oficial
</footer>

</body>
</html>
