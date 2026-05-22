<!DOCTYPE html>
<html>
<head>
<style>
  /* EFECTO LLAMATIVO: CARRUSEL 3D + NEÓN PARPADEANTE */
  body {
    background: #0a0f1e;
    color: #eee;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    padding: 20px;
    margin: 0;
  }
  .card {
    background: #11161f;
    border-radius: 20px;
    padding: 20px;
    margin: 20px auto;
    max-width: 900px;
    box-shadow: 0 0 30px rgba(0,255,255,0.2);
    overflow: hidden;
  }

  /* ========= CARRUSEL 3D LLAMATIVO ========= */
  .tech-showcase {
    margin: 40px 0;
    perspective: 1000px;
    display: flex;
    justify-content: center;
  }
  .carousel-3d {
    position: relative;
    width: 280px;
    height: 280px;
    transform-style: preserve-3d;
    animation: spin3D 12s infinite linear;
  }
  .carousel-item {
    position: absolute;
    width: 100px;
    height: 100px;
    background: rgba(20, 30, 55, 0.9);
    border-radius: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 3rem;
    font-weight: bold;
    box-shadow: 0 0 20px cyan;
    border: 2px solid cyan;
    backdrop-filter: blur(4px);
    left: 50%;
    top: 50%;
    margin-left: -50px;
    margin-top: -50px;
  }
  /* Posiciones 3D */
  .carousel-item:nth-child(1) { transform: rotateY(0deg) translateZ(150px); background: #ff5722; }
  .carousel-item:nth-child(2) { transform: rotateY(60deg) translateZ(150px); background: #2196f3; }
  .carousel-item:nth-child(3) { transform: rotateY(120deg) translateZ(150px); background: #4caf50; }
  .carousel-item:nth-child(4) { transform: rotateY(180deg) translateZ(150px); background: #ffeb3b; color: #000; }
  .carousel-item:nth-child(5) { transform: rotateY(240deg) translateZ(150px); background: #9c27b0; }
  .carousel-item:nth-child(6) { transform: rotateY(300deg) translateZ(150px); background: #e91e63; }

  @keyframes spin3D {
    from { transform: rotateY(0deg); }
    to { transform: rotateY(360deg); }
  }

  /* ========= NEÓN PARPADEANTE ========= */
  .neon-flash {
    text-align: center;
    margin: 30px 0;
    font-size: 2.5rem;
    font-weight: bold;
    font-family: monospace;
    text-transform: uppercase;
    animation: neonPulse 1.2s ease-in-out infinite, colorShift 3s infinite;
    letter-spacing: 4px;
  }
  @keyframes neonPulse {
    0%, 100% { text-shadow: 0 0 5px #fff, 0 0 10px #0ff, 0 0 20px #0ff, 0 0 30px #0ff; opacity: 1; }
    50% { text-shadow: 0 0 2px #fff, 0 0 5px #f0f, 0 0 15px #f0f, 0 0 25px #f0f; opacity: 0.9; }
  }
  @keyframes colorShift {
    0% { color: #ff0066; }
    33% { color: #00ffcc; }
    66% { color: #ffcc00; }
    100% { color: #ff0066; }
  }

  hr {
    border-color: #2a3a5a;
  }
</style>
</head>
<body>
<div class="card">

  <!-- SECCIÓN LLAMATIVA: CARRUSEL 3D + NEÓN -->
  <div class="tech-showcase">
    <div class="carousel-3d">
      <div class="carousel-item">⚛️</div>
      <div class="carousel-item">🐘</div>
      <div class="carousel-item">🎨</div>
      <div class="carousel-item">🔥</div>
      <div class="carousel-item">📱</div>
      <div class="carousel-item">💾</div>
    </div>
  </div>

  <div class="neon-flash">
    🚀 FULL-STACK DEVELOPER ⚡
  </div>

  <!-- Contenido original -->
  <h1 align="center">👋 ¡Hola, soy <span style="color:#4CAF50;">Dalembert Bravo</span>!</h1>
  <h3 align="center">💻 Desarrollador Full-Stack </h3>

  <p align="center">
    <img src="https://komarev.com/ghpvc/?username=Dalembert21&label=Visitas%20al%20perfil&color=0e75b6&style=flat" alt="Dalembert21" />
  </p>

  <hr>

  <h3>🚀 Sobre mí</h3>
  <p>Desarrollador de software Full-Stack especializado en el diseño y construcción de aplicaciones escalables mediante el uso de arquitecturas limpias y patrones como DDD (Domain-Driven Design) y CQRS. Experiencia en la implementación de sistemas basados en eventos con Apache Kafka, optimización de lógica de negocio en el backend y desarrollo de interfaces eficientes en el frontend. Enfoque centrado en la estructura, la mantenibilidad del código y el rendimiento técnico.</p>

  <hr>

  <h3>🧰 Tecnologías y herramientas que uso</h3>

  <h4>💻 Frontend</h4>
  <p>
    <img src="https://skillicons.dev/icons?i=html,css,js,react,angular,figma" />
    <img src="https://img.shields.io/badge/Penpot-000000?style=for-the-badge&logo=penpot&logoColor=white" />
    <img src="https://img.shields.io/badge/Ionic-3880FF?style=for-the-badge&logo=ionic&logoColor=white" />
  </p>

  <h4>⚙️ Backend</h4>
  <p><img src="https://skillicons.dev/icons?i=php,nestjs,nodejs,firebase" /></p>

  <h4>🗃️ Bases de datos</h4>
  <p>
    <img src="https://skillicons.dev/icons?i=mysql,postgresql" />
    <img src="https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white" />
    <img src="https://img.shields.io/badge/Microsoft%20SQL%20Server-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" />
  </p>

  <h4>🧠 Lenguajes</h4>
  <p><img src="https://skillicons.dev/icons?i=java,typescript,php,javascript" /></p>

  <h4>🛠️ Herramientas y colaboración</h4>
  <p><img src="https://skillicons.dev/icons?i=git,github,vscode,androidstudio,postman" /></p>

  <hr>

  <h3>💬 Habilidades blandas</h3>
  <ul>
    <li>🤝 Trabajo en equipo</li>
    <li>🚀 Adaptabilidad y aprendizaje rápido</li>
    <li>🧩 Resolución de problemas</li>
    <li>💬 Comunicación efectiva</li>
  </ul>

  <hr>

  <h3>🏆 Certificaciones y eventos</h3>
  <ul>
    <li>🧠 CCNA: <em>Introduction to Networks</em> – Cisco Networking Academy</li>
    <li>🔐 <em>Introduction to Cybersecurity</em> – Cisco Networking Academy</li>
    <li>🧑‍💻 <em>Ethical Wi-Fi Hacking (Básico)</em></li>
    <li>🎓 <em>VI Congreso de Ciencia de la Computación, Electrónica e Ingeniería Industrial – CSI 2024</em></li>
  </ul>

  <hr>

  <h3>📫 Contáctame</h3>
  <p>📍 Ecuador<br>
  📧 dalembertbravo2@gmail.com<br>
  🔗 <a href="https://www.linkedin.com/in/edalembertbravo/">LinkedIn</a><br>
  💻 <a href="https://github.com/Dalembert21">GitHub</a></p>

  <hr>

  <h3>⚡ Fun fact</h3>
  <blockquote>Me encanta combinar la creatividad del diseño con la lógica del código. Cada proyecto es una nueva oportunidad para aprender algo increíble.</blockquote>

  <hr>

  <p align="center">
    <img src="https://github-readme-stats.vercel.app/api?username=Dalembert21&show_icons=true&theme=tokyonight" height="165" />
    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Dalembert21&layout=compact&theme=tokyonight" height="165" />
  </p>

</div>
</body>
</html>
