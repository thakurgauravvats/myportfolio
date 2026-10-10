
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Gaurav Kumar Thakur - Web Developer and Full Stack Development Learner.">
  <title>Gaurav Kumar Thakur | Web Developer</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
      scroll-padding-top: 80px;
    }

    body {
      font-family: Arial, Helvetica, sans-serif;
      background: #0b1120;
      color: #e5e7eb;
      line-height: 1.7;
      overflow-x: hidden;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    .container {
      width: min(1100px, 90%);
      margin: auto;
    }

    header {
      position: sticky;
      top: 0;
      z-index: 100;
      background: rgba(11, 17, 32, 0.95);
      border-bottom: 1px solid #202a3d;
      backdrop-filter: blur(12px);
    }

    nav {
      min-height: 72px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 20px;
    }

    .logo {
      font-size: 23px;
      font-weight: 800;
      color: #ffffff;
    }

    .logo span {
      color: #60a5fa;
    }

    .nav-links {
      display: flex;
      align-items: center;
      gap: 28px;
    }

    .nav-links a {
      color: #cbd5e1;
      font-size: 14px;
      transition: color 0.2s;
    }

    .nav-links a:hover {
      color: #60a5fa;
    }

    .nav-links .contact-link {
      padding: 9px 16px;
      border: 1px solid #3b82f6;
      border-radius: 8px;
      color: #93c5fd;
    }

    .menu-btn {
      display: none;
      border: 1px solid #334155;
      background: #111b2e;
      color: white;
      padding: 8px 12px;
      border-radius: 7px;
      font-size: 20px;
      cursor: pointer;
    }

    .hero {
      min-height: 570px;
      display: flex;
      align-items: center;
      padding: 90px 0;
    }

    .hero-content {
      max-width: 760px;
    }

    .eyebrow {
      display: inline-block;
      color: #93c5fd;
      background: #142541;
      border: 1px solid #25436a;
      padding: 7px 13px;
      border-radius: 30px;
      font-size: 13px;
      margin-bottom: 24px;
    }

    h1 {
      color: #ffffff;
      font-size: clamp(38px, 7vw, 66px);
      line-height: 1.12;
      letter-spacing: -2px;
      margin-bottom: 20px;
    }

    h1 span {
      color: #60a5fa;
    }

    .hero p {
      max-width: 650px;
      color: #aab7ca;
      font-size: 17px;
      margin-bottom: 30px;
    }

    .buttons {
      display: flex;
      flex-wrap: wrap;
      gap: 13px;
    }

    .btn {
      display: inline-block;
      padding: 12px 21px;
      border-radius: 8px;
      font-weight: 600;
      font-size: 14px;
      transition: transform 0.2s, background 0.2s;
    }

    .btn:hover {
      transform: translateY(-2px);
    }

    .btn-primary {
      background: #3b82f6;
      color: white;
    }

    .btn-primary:hover {
      background: #2563eb;
    }

    .btn-secondary {
      border: 1px solid #334155;
      color: #e2e8f0;
    }

    .btn-secondary:hover {
      background: #172238;
    }

    section {
      padding: 75px 0;
      border-top: 1px solid #1c2739;
    }

    .section-heading {
      margin-bottom: 32px;
    }

    .section-heading h2 {
      font-size: clamp(28px, 4vw, 36px);
      color: #ffffff;
      margin-bottom: 8px;
    }

    .section-heading p {
      color: #94a3b8;
      font-size: 15px;
    }

    .about-text {
      max-width: 800px;
      color: #b8c4d6;
      font-size: 16px;
    }

    .skills-grid,
    .projects-grid,
    .experience-grid {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 18px;
    }

    .card {
      min-width: 0;
      background: #111b2e;
      border: 1px solid #253249;
      border-radius: 13px;
      padding: 23px;
      transition: border-color 0.2s, transform 0.2s;
    }

    .card:hover {
      border-color: #3b82f6;
      transform: translateY(-3px);
    }

    .card h3 {
      color: #f1f5f9;
      font-size: 18px;
      margin-bottom: 8px;
    }

    .card p {
      color: #9eacc0;
      font-size: 14px;
    }

    .skill-tag {
      display: inline-block;
      background: #192943;
      color: #bfdbfe;
      border: 1px solid #2b4568;
      border-radius: 7px;
      padding: 8px 13px;
      margin: 5px 5px 5px 0;
      font-size: 14px;
    }

    .education-card {
      max-width: 750px;
    }

    .education-card .muted {
      color: #93a4bb;
      font-size: 14px;
      margin-top: 5px;
    }

    .contact-content {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 30px;
      align-items: start;
    }

    .contact-details {
      display: grid;
      gap: 14px;
    }

    .contact-item {
      padding: 15px 18px;
      border: 1px solid #253249;
      background: #111b2e;
      border-radius: 10px;
      overflow-wrap: anywhere;
    }

    .contact-item strong {
      display: block;
      color: #93c5fd;
      font-size: 13px;
      margin-bottom: 4px;
    }

    .contact-item a,
    .contact-item span {
      color: #e2e8f0;
      font-size: 14px;
    }

    .contact-item a:hover {
      color: #60a5fa;
    }

    .contact-note {
      color: #aab7ca;
      padding-top: 8px;
    }

    footer {
      border-top: 1px solid #1c2739;
      padding: 25px 0;
      text-align: center;
      color: #8190a5;
      font-size: 13px;
    }

    @media (max-width: 760px) {
      .menu-btn {
        display: block;
      }

      .nav-links {
        display: none;
        position: absolute;
        top: 72px;
        left: 0;
        right: 0;
        padding: 20px 5%;
        background: #0b1120;
        border-bottom: 1px solid #253249;
        flex-direction: column;
        align-items: stretch;
        gap: 18px;
      }

      .nav-links.open {
        display: flex;
      }

      .nav-links .contact-link {
        text-align: center;
      }

      .hero {
        min-height: auto;
        padding: 85px 0;
      }

      .hero p {
        font-size: 15px;
      }

      section {
        padding: 58px 0;
      }

      .skills-grid,
      .projects-grid,
      .experience-grid,
      .contact-content {
        grid-template-columns: 1fr;
      }

      h1 {
        letter-spacing: -1.3px;
      }
    }

    @media (prefers-reduced-motion: reduce) {
      html {
        scroll-behavior: auto;
      }

      *,
      *::before,
      *::after {
        transition: none !important;
      }
    }
  </style>
</head>

<body>
  <header>
    <nav class="container">
      <a class="logo" href="#home">Gaurav<span>.</span></a>

      <button
        class="menu-btn"
        id="menuBtn"
        aria-label="Open navigation menu"
        aria-expanded="false"
        aria-controls="navLinks"
      >☰</button>

      <div class="nav-links" id="navLinks">
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#projects">Projects</a>
        <a href="#education">Education</a>
        <a class="contact-link" href="#contact">Contact Me</a>
      </div>
    </nav>
  </header>

  <main>
    <section class="hero" id="home">
      <div class="container">
        <div class="hero-content">
          <span class="eyebrow">Web Developer · Full Stack Learner</span>

          <h1>
            Hi, I'm Gaurav<br>
            <span>Kumar Thakur.</span>
          </h1>

          <p>
            I'm a BCA student interested in web development and building
            useful, user-friendly websites. I'm currently improving my
            frontend skills and learning full-stack development.
          </p>

          <div class="buttons">
            <a class="btn btn-primary" href="#projects">View My Projects</a>
            <a class="btn btn-secondary" href="#contact">Get In Touch</a>
          </div>
        </div>
      </div>
    </section>

    <section id="about">
      <div class="container">
        <div class="section-heading">
          <h2>About Me</h2>
          <p>A little about my background and interests.</p>
        </div>

        <p class="about-text">
          I'm pursuing a Bachelor of Computer Applications (BCA) in
          Artificial Intelligence and Data Science at Vivekananda Global
          University, Jaipur. I enjoy learning web technologies and turning
          ideas into working projects. My current focus is on strengthening
          my frontend development skills while learning backend development
          to become a full-stack developer.
        </p>
      </div>
    </section>

    <section id="skills">
      <div class="container">
        <div class="section-heading">
          <h2>My Skills</h2>
          <p>Technologies I'm learning and working with.</p>
        </div>

        <div class="skills-grid">
          <div class="card">
            <h3>Frontend</h3>
            <p>Building website layouts and user interfaces.</p>
            <div>
              <span class="skill-tag">HTML</span>
              <span class="skill-tag">CSS</span>
              <span class="skill-tag">JavaScript</span>
              <span class="skill-tag">React.js</span>
            </div>
          </div>

          <div class="card">
            <h3>Tools</h3>
            <p>Tools I use while learning and developing projects.</p>
            <div>
              <span class="skill-tag">Git</span>
              <span class="skill-tag">GitHub</span>
              <span class="skill-tag">VS Code</span>
            </div>
          </div>

          <div class="card">
            <h3>Currently Learning</h3>
            <p>Developing my skills to build complete web applications.</p>
            <div>
              <span class="skill-tag">Full Stack Development</span>
              <span class="skill-tag">Backend Development</span>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="projects">
      <div class="container">
        <div class="section-heading">
          <h2>My Projects</h2>
          <p>Some projects I've worked on.</p>
        </div>

        <div class="projects-grid">
          <div class="card">
            <h3>JOB TRACK</h3>
            <p>Web development project.</p>
          </div>

          <div class="card">
            <h3>Plastic Waste Management</h3>
            <p>Plastic waste management project.</p>
          </div>

          <div class="card">
            <h3>EcoTrack</h3>
            <p>Environmental sustainability project.</p>
          </div>
        </div>
      </div>
    </section>

    <section id="experience">
      <div class="container">
        <div class="section-heading">
          <h2>Internship Experience</h2>
          <p>My internship learning experience.</p>
        </div>

        <div class="experience-grid">
          <div class="card">
            <h3>Uptoskill</h3>
            <p>Web Development Internship</p>
          </div>

          <div class="card">
            <h3>SkillCraft</h3>
            <p>Web Development Internship</p>
          </div>

          <div class="card">
            <h3>Career Goal</h3>
            <p>Continuously learning and growing as a web developer.</p>
          </div>
        </div>
      </div>
    </section>

    <section id="education">
      <div class="container">
        <div class="section-heading">
          <h2>Education</h2>
          <p>My academic background.</p>
        </div>

        <div class="card education-card">
          <h3>Bachelor of Computer Applications (BCA)</h3>
          <p>Artificial Intelligence and Data Science</p>
          <p class="muted">Vivekananda Global University, Jaipur</p>
          <p class="muted">2024 – 2027 (Expected)</p>
        </div>
      </div>
    </section>

    <section id="contact">
      <div class="container">
        <div class="section-heading">
          <h2>Let's Connect</h2>
          <p>Feel free to reach out for opportunities and collaborations.</p>
        </div>

        <div class="contact-content">
          <div>
            <h3>Get in touch</h3>
            <p class="contact-note">
              I'm interested in web development opportunities where I can
              learn, contribute, and improve my skills.
            </p>
          </div>

          <div class="contact-details">
            <div class="contact-item">
              <strong>Email</strong>
              <a href="mailto:gkt7565@gmail.com">gkt7565@gmail.com</a>
            </div>

            <div class="contact-item">
              <strong>Phone</strong>
              <a href="tel:7991187225">7991187225</a>
            </div>

            <div class="contact-item">
              <strong>Location</strong>
              <span>Jaipur, Rajasthan, India</span>
            </div>

            <div class="contact-item">
              <strong>GitHub</strong>
              <a href="https://github.com/thakurgauravvats"
                 target="_blank" rel="noopener noreferrer">
                github.com/thakurgauravvats
              </a>
            </div>

            <div class="contact-item">
              <strong>LinkedIn</strong>
              <a href="https://www.linkedin.com/in/gaurav-thakur-b74782323/"
                 target="_blank" rel="noopener noreferrer">
                View LinkedIn Profile
              </a>
            </div>
          </div>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="container">
      <p>© <span id="year"></span> Gaurav Kumar Thakur. All rights reserved.</p>
    </div>
  </footer>

  <script>
    const menuBtn = document.getElementById("menuBtn");
    const navLinks = document.getElementById("navLinks");

    menuBtn.addEventListener("click", () => {
      const isOpen = navLinks.classList.toggle("open");
      menuBtn.setAttribute("aria-expanded", isOpen);
      menuBtn.setAttribute(
        "aria-label",
        isOpen ? "Close navigation menu" : "Open navigation menu"
      );
      menuBtn.textContent = isOpen ? "✕" : "☰";
    });

    navLinks.querySelectorAll("a").forEach((link) => {
      link.addEventListener("click", () => {
        navLinks.classList.remove("open");
        menuBtn.setAttribute("aria-expanded", "false");
        menuBtn.setAttribute("aria-label", "Open navigation menu");
        menuBtn.textContent = "☰";
      });
    });

    document.getElementById("year").textContent =
      new Date().getFullYear();
  </script>
</body>
</html>
