<template>
  <main class="portfolio">
    <header class="navbar">
      <a class="logo" href="#home">ZM.</a>

      <nav>
        <a href="#about">About</a>
        <a href="#projects">Projects</a>
        <a href="#skills">Skills</a>
        <a class="contact-link" href="#contact">Contact ↗</a>
      </nav>
    </header>

    <section id="home" class="hero">
      <p class="eyebrow">● COMPUTER ENGINEERING STUDENT</p>

      <h1>
        Hi, I'm Zander.<br />
        I build <span>my future.</span>
      </h1>

      <p class="intro">
        A computer engineering student learning web development,
        exploring technology, and turning ideas into practical projects.
      </p>

      <div class="actions">
        <a class="button primary" href="#projects">Explore my work ↗</a>
        <a class="button secondary" href="#contact">Get in touch</a>
      </div>

      <p class="note">Currently learning web development from the ground up.</p>
    </section>

    <section id="about" class="section">
      <p class="eyebrow">01 / ABOUT</p>
      <h2>A little about <span>me.</span></h2>

      <div class="about-grid">
        <h3>
          I'm a Computer Engineering student interested in how technology
          can solve real problems.
        </h3>

        <div class="muted">
          <p>
            I'm starting my web development journey by learning the
            fundamentals and applying them through hands-on projects.
          </p>
          <p>
            My interests include electronics, programming, problem-solving,
            and building useful technology solutions.
          </p>

          <div class="info-row">
            <span>EDUCATION</span>
            <span>Computer Engineering</span>
          </div>
          <div class="info-row">
            <span>FOCUS</span>
            <span>Engineering & Technology</span>
          </div>
          <div class="info-row">
            <span>CURRENT GOAL</span>
            <span>Learn and build consistently</span>
          </div>
        </div>
      </div>
    </section>

    <section id="projects" class="section">
      <p class="eyebrow">02 / SELECTED WORK</p>
      <h2>Projects in <span>progress.</span></h2>

      <div class="project-grid">
        <article class="project-card">
          <div class="project-art circuit-art">
            <div class="circuit-box">
              <span>AC</span>
              <strong>12V DC</strong>
              <span>DC</span>
            </div>
          </div>
          <p class="eyebrow">ELECTRONICS · ENGINEERING</p>
          <h3>Electronics Project</h3>
          <p class="muted">
            An electronics project focused on circuit concepts and practical
            engineering applications.
          </p>
          <div class="tags">
            <span>Electronics</span>
            <span>Circuit Design</span>
            <span>Engineering</span>
          </div>
        </article>

        <article class="project-card">
          <div class="project-art code-art">
            <div class="code-window">
              <div class="window-bar">● ● ● &nbsp; portfolio.vue</div>
              <pre><code>const portfolio = {
  name: 'Zander',
  learning: true
}</code></pre>
            </div>
          </div>
          <p class="eyebrow">WEB DEVELOPMENT · LEARNING</p>
          <h3>Website Development</h3>
          <p class="muted">
            A website development project for practicing frontend design
            and building functional web experiences.
          </p>
          <div class="tags">
            <span>HTML & CSS</span>
            <span>JavaScript</span>
            <span>Vue.js</span>
          </div>
        </article>

        <article class="project-card">
          <div class="project-art portfolio-art">
            <div class="mini-logo">ZM.</div>
            <span>MY DIGITAL SPACE</span>
          </div>
          <p class="eyebrow">PERSONAL PROJECT · LEARNING</p>
          <h3>Personal Portfolio</h3>
          <p class="muted">
            This portfolio website, built while learning Vue.js, CSS,
            and the fundamentals of web development.
          </p>
          <div class="tags">
            <span>Vue.js</span>
            <span>Vite</span>
            <span>CSS</span>
          </div>
        </article>
      </div>
    </section>

    <section id="skills" class="section">
      <p class="eyebrow">03 / TOOLKIT</p>
      <h2>Skills & <span>learning.</span></h2>
      <p class="muted skill-intro">
        My starting point. These skills will develop through study,
        practice, and real projects.
      </p>

      <div class="skills-list">
        <div>01 <span>Problem Solving</span></div>
        <div>02 <span>Critical Thinking</span></div>
        <div>03 <span>Electronics Fundamentals</span></div>
        <div>04 <span>Circuit Analysis</span></div>
        <div>05 <span>HTML & CSS — Learning</span></div>
        <div>06 <span>JavaScript — Learning</span></div>
        <div>07 <span>Python — Learning</span></div>
        <div>08 <span>Vue.js — Learning</span></div>
        <div>09 <span>Django — Learning</span></div>
      </div>
    </section>

    <section id="contact" class="contact-section">
      <p class="eyebrow">04 / CONTACT</p>
      <h2>Let's connect<span>.</span></h2>
      <p class="muted">
        Have a question or want to connect? Feel free to reach out.
      </p>
      <a class="button primary" href="mailto:">Email me ↗</a>

      <div class="contact-footer">
        <span>OPEN TO LEARNING OPPORTUNITIES</span>
        <a href="#home">BACK TO TOP ↑</a>
      </div>
    </section>

    <footer class="footer">
      <a class="logo" href="#home">ZM.</a>
      <p>Designed and built while learning, one step at a time.</p>
      <p>© 2026 Zander Mamuad</p>
    </footer>
  </main>
</template>