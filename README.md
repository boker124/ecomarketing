<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>ECOMARKETING - Marketing & Producción Sustentable</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --azul-claro: #a9d6ff;
      --marron: #7b4f3a;
      --oliva: #7a8b3b;
      --gris-claro: #f5f5f7;
      --texto: #222;
      --accent: #ffd166;
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;font-family:'Poppins',system-ui,Arial; color:var(--texto);background:linear-gradient(180deg, #ffffff 0%, var(--gris-claro) 100%)}
    a{color:inherit;text-decoration:none}

    /* Layout */
    .container{max-width:1200px;margin:40px auto;padding:28px}
    header{display:flex;align-items:center;justify-content:space-between;gap:20px}
    .logo{display:flex;align-items:center;gap:14px}
    .logo img{width:120px;height:120px;object-fit:cover;border-radius:12px;border:3px solid rgba(0,0,0,0.06);box-shadow:0 6px 18px rgba(0,0,0,0.08)}
    .brand{display:flex;flex-direction:column}
    .brand h1{margin:0;font-size:36px;color:var(--marron);letter-spacing:0.6px}
    .brand p{margin:0;font-size:14px;color:#555}

    nav a{margin-left:18px;padding:8px 12px;border-radius:8px;font-weight:600}
    nav a:hover{background:rgba(0,0,0,0.04)}

    /* Hero */
    .hero{display:grid;grid-template-columns:1fr 420px;gap:30px;align-items:center;margin-top:28px}
    .hero-card{background:linear-gradient(180deg, rgba(255,255,255,0.9), #ffffff);padding:28px;border-radius:18px;box-shadow:0 12px 40px rgba(12,18,22,0.06);border:1px solid rgba(0,0,0,0.03)}
    .kicker{display:inline-block;padding:6px 10px;border-radius:999px;background:var(--azul-claro);color:#03396c;font-weight:700;margin-bottom:12px}
    .hero-card h2{margin:8px 0 12px;font-size:34px;color:var(--marron)}
    .hero-card p.lead{margin:0 0 18px;line-height:1.5}
    .cta{display:inline-block;padding:12px 18px;border-radius:12px;background:var(--oliva);color:white;font-weight:700}

    .hero-aside{border-radius:12px;padding:18px;background:linear-gradient(180deg,var(--azul-claro),white);text-align:center}
    .hero-aside img{width:100%;border-radius:10px;box-shadow:0 10px 30px rgba(0,0,0,0.08)}

    /* Sections */
    section{margin-top:30px}
    .grid-3{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
    .card{background:white;padding:18px;border-radius:12px;border:1px solid rgba(0,0,0,0.03);box-shadow:0 8px 24px rgba(5,10,10,0.03);overflow:hidden}
    .card img{width:100%;height:180px;object-fit:cover;border-radius:8px;margin-bottom:12px;border:2px solid rgba(0,0,0,0.03)}
    .card h3{margin:6px 0;color:var(--marron)}
    .card p{margin:0;color:#444}

    /* Catalog */
    .catalog{display:flex;gap:18px;flex-wrap:wrap}
    .product{flex:1 1 320px;background:linear-gradient(180deg,#fff, #fcfcfc);padding:18px;border-radius:12px;border:1px solid rgba(0,0,0,0.04)}
    .price{font-weight:800;color:var(--oliva);font-size:20px}

    footer{margin-top:40px;padding:20px;border-top:1px solid rgba(0,0,0,0.04);text-align:center;color:#666}

    /* Frames & animations */
    .frame{padding:12px;border-radius:12px;border:2px solid rgba(0,0,0,0.04);background:linear-gradient(180deg, rgba(255,255,255,0.6), rgba(255,255,255,0.4));}
    .fade-up{opacity:0;transform:translateY(18px);animation:fadeUp .8s forwards}
    .delay-1{animation-delay:0.12s}
    .delay-2{animation-delay:0.24s}
    .delay-3{animation-delay:0.36s}
    @keyframes fadeUp{to{opacity:1;transform:none}}

    .img-frame{display:block;border-radius:10px;overflow:hidden;transition:transform .45s ease, box-shadow .45s ease;cursor:pointer}
    .img-frame:hover{transform:translateY(-8px) scale(1.02);box-shadow:0 18px 60px rgba(0,0,0,0.12)}

    /* Modal */
    .modal {
      display: none; 
      position: fixed; 
      z-index: 1000; 
      padding-top: 60px; 
      left: 0; 
      top: 0; 
      width: 100%; 
      height: 100%; 
      overflow: auto; 
      background-color: rgba(0,0,0,0.7);
    }
    .modal-content {
      margin: auto;
      display: block;
      max-width: 90%;
      border-radius: 10px;
      box-shadow: 0 12px 40px rgba(0,0,0,0.5);
    }
  </style>
</head>
<body>
  <div class="container">
    <header class="fade-up">
      <div class="logo">
        <img src="https://i.postimg.cc/vZfG9jH2/Whats-App-Image-2025-09-17-at-3-55-33-PM.jpg" alt="Logo ECOMARKETING">
        <div class="brand">
          <h1>ECOMARKETING</h1>
          <p>Marketing & Producción Sustentable</p>
        </div>
      </div>
      <nav>
        <a href="#mision">Misión</a>
        <a href="#vision">Visión</a>
        <a href="#proceso">Proceso</a>
        <a href="#catalogo">Catálogo</a>
      </nav>
    </header>

    <main>
      <div class="hero">
        <div class="hero-card frame fade-up delay-1">
          <span class="kicker">Sustentable · Local · Creativo</span>
          <h2>Devolvemos vida a la ropa. Promocionamos tu negocio.</h2>
          <p class="lead">En ECOMARKETING combinamos procesos responsables de recolección y transformación con estrategias de marketing digital para darle una segunda vida a prendas y posicionar negocios locales en redes.</p>
          <a class="cta" href="#catalogo">Ver Servicios</a>
        </div>

        <aside class="hero-aside frame fade-up delay-2">
          <img src="https://i.postimg.cc/dV5XXj1m/Opera-Captura-de-pantalla-2025-09-17-161616-www-canva-com.png" alt="Nuestro catálogo" class="img-frame">
          <p style="margin-top:10px;font-weight:600">Catálogo destacado</p>
        </aside>
      </div>

      <!-- Misión y Visión -->
      <section id="mision" class="fade-up delay-3">
        <div class="card frame">
          <h3>Misión</h3>
          <p>Somos una empresa centrada en comercializar y posicionar nuestra empresa como lo es <strong>ECOMARKETING</strong>. Nosotros, como empresa enfocada en marketing digital, garantizamos por medio de nuestras redes sociales que nuestros métodos son monitoreados y empleados adecuadamente. Mostramos que gracias a nuestros rigurosos procesos de recolección, transformación, higienización y comercialización podemos darle a las prendas una segunda nueva vida útil y poner en circulación ropa que ya había cumplido su ciclo. Abordando y enfatizando en las personas temas como la conservación de los recursos ambientales.</p>
        </div>
      </section>

      <section id="vision" class="fade-up delay-2" style="margin-top:14px">
        <div class="card frame">
          <h3>Visión</h3>
          <p>Para <strong>2030</strong> seremos una empresa reconocida municipalmente por su alto compromiso con la satisfacción del cliente así como con el medio ambiente gracias a nuestras políticas, las cuales buscan concientizar acerca de las problemáticas ambientales que produce la industria de la moda.</p>
        </div>
      </section>

      <!-- Proceso de Producción -->
      <section id="proceso">
        <h2 style="color:var(--marron);margin-top:22px">Proceso de Producción (Prestación de Servicios)</h2>
        <div class="grid-3" style="margin-top:12px">

          <div class="card frame fade-up">
            <img src="https://i.postimg.cc/fTMP5rKg/ada99ede-6546-4d3d-9963-6ad45d28a3a0.jpg" alt="Reunión con el cliente" class="img-frame modal-img">
            <h3>Reunión con el cliente</h3>
            <p>Conversamos con un cliente dueño de una barbería para conocer sus ideas. Tendremos en cuenta qué servicios ofrece y cómo podemos ayudarle a promocionar su negocio con estrategias de marketing.</p>
          </div>

          <div class="card frame fade-up delay-1">
            <img src="https://i.postimg.cc/xj55jTvt/0c15b98d-0bd6-4eda-bf04-2cd3cd29c972.jpg" alt="Análisis del mercado" class="img-frame modal-img">
            <h3>Análisis del mercado</h3>
            <p>Analizamos otras barberías de la zona y en redes sociales para conocer qué servicios ofrecen, cómo se promocionan y qué precios manejan. Investigamos qué buscan los clientes para lograr que la barbería destaque.</p>
          </div>

          <div class="card frame fade-up delay-2">
            <img src="https://i.postimg.cc/TwCbx1zb/f77cb90c-9b14-4a63-bd74-bce891e4f062.jpg" alt="Diseño de estrategia" class="img-frame modal-img">
            <h3>Diseño de la estrategia</h3>
            <p>Diseñamos una estrategia de marketing enfocada en atraer más clientes a la barbería, con mensajes claros y canales adecuados según el público objetivo.</p>
          </div>

          <div class="card frame fade-up delay-3">
            <img src="https://i.postimg.cc/cJ1YbfjW/ece9ff04-aaeb-45c8-8786-f201de38a109.jpg" alt="Creación de contenido" class="img-frame modal-img">
            <h3>Creación de contenido</h3>
            <p>Creamos contenido visual atractivo para redes sociales: fotos de cortes, reels mostrando el ambiente y material que siga la estética de la barbería.</p>
          </div>

          <div class="card frame fade-up delay-1">
            <img src="https://i.postimg.cc/C1qKP1FY/f69a5127-b415-4c74-8148-db0f15c792cd.jpg" alt="Contenido adicional" class="img-frame modal-img">
            <h3>Contenido extra</h3>
            <p>Generamos variaciones del contenido para historias, posts fijos y anuncios según las métricas de interacción.</p>
          </div>

          <div class="card frame fade-up delay-2">
            <img src="https://i.postimg.cc/YSJrWHQP/de890866-7eaa-40b1-b8c2-813b47246e79.jpg" alt="Publicación" class="img-frame modal-img">
            <h3>Publicación de la publicidad</h3>
            <p>Publicamos el contenido en las redes sociales de la barbería y observamos cómo reacciona el público, ajustando según resultados.</p>
          </div>

        </div>
      </section>

      <!-- Catálogo -->
      <section id="catalogo" style="margin-top:28px">
        <h2 style="color:var(--marron)">Nuestro Catálogo</h2>
        <div class="catalog" style="margin-top:12px">

          <div class="product frame fade-up">
            <img src="https://i.postimg.cc/W4Q9LWPr/30a2cc39-9917-428d-8daa-5c357ec29910.jpg" alt="Diseño de logo" class="img-frame modal-img" style="width:100%;border-radius:8px;margin-bottom:12px">
            <h3>Diseño de Logo</h3>
            <p>Diseño profesional de logotipos que representen la identidad de tu marca.</p>
            <p class="price">$150.000</p>
            <p style="font-size:13px;color:#666;margin-top:8px">Ideal para negocios que buscan venta online.</p>
          </div>

          <div class="product frame fade-up delay-1">
            <img src="https://i.postimg.cc/dV5XXj1m/Opera-Captura-de-pantalla-2025-09-17-161616-www-canva-com.png" alt="Gestión redes" class="img-frame modal-img" style="width:100%;border-radius:8px;margin-bottom:12px">
            <h3>Gestión & Contenido</h3>
            <p>Creamos y publicamos contenido estratégico en redes sociales para aumentar tu alcance y ventas.</p>
            <p class="price">$90.000</p>
            <p style="font-size:13px;color:#666;margin-top:8px">Paquete pensado para emprendedores.</p>
          </div>

        </div>
      </section>

    </main>

    <footer class="fade-up" style="margin-top:28px">
      <p>© ECOMARKETING 2025 · Marketing sostenible · Hecho con intención</p>
      <p style="font-size:13px;color:#888;margin-top:6px">Diseñado con paleta: azul claro, marrón y verde oliva.</p>
    </footer>
  </div>

  <!-- Modal dinámico -->
  <script>
    document.querySelectorAll('.modal-img, .hero-aside img').forEach(img => {
      img.addEventListener('click', function() {
        const modal = document.createElement('div');
        modal.classList.add('modal');
        modal.innerHTML = `<img src="${this.src}" class="modal-content">`;
        modal.addEventListener('click', () => modal.remove());
        document.body.appendChild(modal);
        modal.style.display = 'block';
      });
    });
  </script>
</body>
</html>
