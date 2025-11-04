<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Sivasubramaniyan E | Portfolio</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }

    body {
      background-color: #f8f9fa;
      color: #333;
      scroll-behavior: smooth;
    }

    header {
      background-color: #ffffff;
      padding: 20px 0;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
      position: fixed;
      width: 100%;
      z-index: 10;
    }

    nav {
      width: 90%;
      margin: auto;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    nav h1 {
      font-size: 24px;
      color: #007bff;
    }

    nav ul {
      list-style: none;
      display: flex;
    }

    nav ul li {
      margin: 0 15px;
    }

    nav ul li a {
      text-decoration: none;
      color: #333;
      font-weight: 500;
      transition: 0.3s;
    }

    nav ul li a:hover {
      color: #007bff;
    }

    section {
      padding: 100px 10%;
      min-height: 100vh;
    }

    .home {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
    }

    .home h2 {
      font-size: 40px;
      margin-bottom: 10px;
      color: #007bff;
    }

    .home p {
      font-size: 18px;
      max-width: 600px;
    }

    .about, .skills, .education, .contact {
      margin-top: 50px;
    }

    h2.section-title {
      text-align: center;
      margin-bottom: 30px;
      color: #007bff;
      font-size: 28px;
    }

    .skills ul {
      display: flex;
      justify-content: center;
      gap: 30px;
      flex-wrap: wrap;
      list-style: none;
    }

    .skills li {
      background: #e9ecef;
      padding: 10px 20px;
      border-radius: 20px;
      font-weight: 500;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }

    .education p, .contact p {
      text-align: center;
      font-size: 18px;
    }

    .contact-info {
      text-align: center;
      margin-top: 20px;
    }

    .contact-info a {
      color: #007bff;
      text-decoration: none;
      font-weight: 500;
    }

    footer {
      background: #007bff;
      color: white;
      text-align: center;
      padding: 15px 0;
      margin-top: 50px;
    }

    /* Animation */
    .fade-in {
      opacity: 0;
      transform: translateY(30px);
      transition: all 0.8s ease;
    }
    .fade-in.visible {
      opacity: 1;
      transform: translateY(0);
    }
  </style>
</head>
<body>
  <header>
    <nav>
      <h1>Siva.</h1>
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#education">Education</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section id="home" class="home fade-in">
    <h2>Hi, I'm Sivasubramaniyan E</h2>
    <p>A passionate Computer Science student at R P Sarathy Institute of Technology, Salem.</p>
  </section>

  <section id="about" class="about fade-in">
    <h2 class="section-title">About Me</h2>
    <p style="text-align:center; max-width:600px; margin:auto;">
      I am Sivasubramaniyan.E, pursuing Computer Science and Engineering at R P Sarathy Institute of Technology, Salem.
      I have a keen interest in web development and programming using HTML and Python.
    </p>
  </section>

  <section id="skills" class="skills fade-in">
    <h2 class="section-title">Skills</h2>
    <ul>
      <li>HTML</li>
      <li>Python</li>
    </ul>
  </section>

  <section id="education" class="education fade-in">
    <h2 class="section-title">Education</h2>
    <p>HSC – 67%</p>
    <p>SSLC – 62.2%</p>
  </section>

  <section id="contact" class="contact fade-in">
    <h2 class="section-title">Contact</h2>
    <div class="contact-info">
      <p>Email: <a href="mailto:sivakd40081@gmail.com">sivakd40081@gmail.com</a></p>
      <p>Phone: <a href="tel:+916385369922">+91 63853 69922</a></p>
    </div>
  </section>

  <footer>
    <p>© 2025 Sivasubramaniyan E | All Rights Reserved</p>
  </footer>

  <script>
    // Fade-in animation on scroll
    const elements = document.querySelectorAll('.fade-in');
    function reveal() {
      elements.forEach(el => {
        const rect = el.getBoundingClientRect();
        if (rect.top < window.innerHeight - 100) {
          el.classList.add('visible');
        }
      });
    }
    window.addEventListener('scroll', reveal);
    reveal();
  </script>
</body>
</html>
