<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Kuromi Portfolio</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <style>
    /* GOOGLE FONT */
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap');

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }

    body {
      background: linear-gradient(135deg, #1a001f, #2d0033);
      color: #fff;
    }

    /* NAVBAR */
    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 15px 30px;
      background: #0f0014;
      position: fixed;
      width: 100%;
      top: 0;
      z-index: 100;
    }

    nav h1 {
      color: #ff7ad9;
      font-size: 22px;
    }

    nav ul {
      list-style: none;
      display: flex;
      gap: 20px;
    }

    nav ul li {
      cursor: pointer;
      transition: 0.3s;
    }

    nav ul li:hover {
      color: #ff7ad9;
    }

    /* SECTIONS */
    section {
      min-height: 100vh;
      padding: 100px 30px;
      display: none;
    }

    section.active {
      display: block;
    }

    h2 {
      color: #ff7ad9;
      margin-bottom: 15px;
    }

    /* HOME */
    .home {
      text-align: center;
    }

    .home img {
      width: 180px;
      margin: 20px 0;
    }

    .home h3 {
      font-weight: 300;
    }

    /* SKILLS */
    .skills-list {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
      gap: 15px;
      margin-top: 20px;
    }

    .skill {
      background: #24002b;
      padding: 15px;
      border-radius: 10px;
      text-align: center;
    }

    /* PROJECTS */
    .project {
      background: #24002b;
      padding: 20px;
      border-radius: 10px;
      margin-bottom: 15px;
    }

    /* CONTACT */
    .contact a {
      color: #ff6bff;
      text-decoration: none;
      font-weight: bold;
    }

    .contact a:hover {
      color: #c77dff;
    }

    footer {
      text-align: center;
      padding: 20px;
      background: #0f0014;
    }
  </style>
</head>

<body>

  <!-- NAVIGATION -->
  <nav>
    <ul>
      <li onclick="showSection('home')">Home</li>
      <li onclick="showSection('about')">About</li>
      <li onclick="showSection('skills')">Skills</li>
      <li onclick="showSection('projects')">Projects</li>
      <li onclick="showSection('contact')">Contact</li>
    </ul>
  </nav>

  <!-- HOME -->
  <section id="home" class="home active">
    <h2>Hello, I'm Joemilyn Mabini Lizano 💜</h2>
    <h3>Web Developer | Designer | Student </h3>
    <img src="https://uploads.onecompiler.io/43zv5aqkm/449yu5jbh/Messenger_creation_E80B527D-7452-4829-A24B-52E35A01F277.jpeg" alt="picture">
    <p>Welcome to my personal portfolio website.</p>
  </section>

  <!-- ABOUT -->
  <section id="about">
    <h2>About Me</h2>
    <p>
      I’m a beginner web developer who loves creating cute and creative websites. I enjoy learning new things and improving my skills.
    </p>
  </section>

  <!-- SKILLS -->
  <section id="skills">
    <h2>My Skills</h2>
    <div class="skills-list">
      <div class="skill">HTML</div>
      <div class="skill">CSS</div>
      <div class="skill">JavaScript</div>
      <div class="skill">Responsive Design</div>
      <div class="skill">UI Design</div>
    </div>
  </section>

  <!-- PROJECTS -->
  <section id="projects">
    <h2>Projects</h2>

    <div class="project">
      <h3>Project 1</h3>
      <p>A sample project showcasing my development skills with modern design.</p>
    </div>

    <div class="project">
      <h3>Project 2</h3>
      <p>Another project built with creativity and a focus on user-friendly interface.</p>
    </div>
  </section>

  <!-- CONTACT -->
    <section id="contact" class="contact">
    <h2>Contact</h2>
    <p>Feel free to reach out:</p>
    <p>Email: <a href="mailto:joemilynmabinilizano@gmail.com">joemilynmabinilizano@gmail.com</a></p>
  </section>

  <footer>
    <p>© 2026 All Rigths Reserved 💜</p>
  </footer>

  <!-- JAVASCRIPT -->
  <script>
    function showSection(sectionId) {
      document.querySelectorAll('section').forEach(section => {
        section.classList.remove('active');
      });
      document.getElementById(sectionId).classList.add('active');
      window.scrollTo(0, 0);
    }
  </script>

</body>
</html>
