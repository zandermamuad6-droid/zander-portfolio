
<template>
  <main>
    <!-- Navigation -->
    <header class="navbar">
      <a class="logo" href="#home">ZM.</a>

      <nav class="nav-links">
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#projects">Projects</a>
        <a href="#skills">Skills</a>
        <a href="#contact">Contact</a>
      </nav>

      <a class="nav-button" href="#contact">Let's Talk <span>↗</span></a>
    </header>

    <!-- Hero -->
    <section id="home" class="hero section-container">
      <div class="hero-content">
        <p class="eyebrow"><span class="status-dot"></span> AVAILABLE FOR OPPORTUNITIES</p>

        <h1>
          Hi, I'm <span class="gradient-text">Zander.</span><br />
          I build things for<br />
          the <span class="gradient-text">digital world.</span>
        </h1>

        <p class="hero-description">
          An aspiring developer passionate about creating useful,
          modern, and user-friendly digital experiences.
        </p>

        <div class="hero-actions">
          <a class="button button-primary" href="#projects">Explore My Work <span>↗</span></a>
          <a class="button button-secondary" href="#about">More About Me</a>
        </div>

        <div class="hero-note">
          <span class="note-line"></span>
          <span>Designed and built while learning, one step at a time.</span>
        </div>
      </div>

      <div class="hero-visual">
        <div class="visual-glow"></div>
        <div class="visual-card">
          <div class="visual-card-top">
            <span class="window-dot"></span>
            <span class="window-dot"></span>
            <span class="window-dot"></span>
            <span class="visual-label">MY WORKSPACE</span>
          </div>

          <div class="code-display">
            <p><span class="code-purple">const</span> developer = {</p>
            <p class="code-indent">name: <span class="code-green">'Zander'</span>,</p>
            <p class="code-indent">focus: <span class="code-green">'Web Development'</span>,</p>
            <p class="code-indent">learning: <span class="code-green">'Every day'</span>,</p>
            <p class="code-indent">building: <span class="code-green">'The future'</span></p>
            <p>};</p>
            <p class="code-comment">// Always keep learning.</p>
          </div>

          <div class="visual-card-bottom">
            <span class="status-dot"></span>
            Currently learning & building
          </div>
        </div>

        <div class="floating-badge badge-top">✦ Creative mindset</div>
        <div class="floating-badge badge-bottom">⌘ Developer in progress</div>
      </div>
    </section>

    <!-- About -->
    <section id="about" class="section-container section-block">
      <div class="section-heading">
        <p class="eyebrow">01 / ABOUT ME</p>
        <h2>A little about <span class="gradient-text">my journey.</span></h2>
      </div>

      <div class="about-grid">
        <div class="about-card about-intro">
          <span class="card-icon">✳</span>
          <h3>Curious by nature.<br />Developer by passion.</h3>
          <p>
            I'm learning how to turn ideas into working projects through
            coding, experimentation, and consistent practice.
          </p>
        </div>

        <div class="about-card">
          <span class="small-label">MY APPROACH</span>
          <h3>Learn. Build. Improve.</h3>
          <p>
            I believe that progress comes from staying curious,
            solving problems, and being willing to start from zero.
          </p>
        </div>

        <div class="about-card">
          <span class="small-label">MY GOAL</span>
          <h3>Create meaningful work.</h3>
          <p>
            My goal is to grow my technical skills, build real-world
            projects, and become a capable developer.
          </p>
        </div>
      </div>
    </section>

    <!-- Projects -->
    <section id="projects" class="section-container section-block">
      <div class="section-heading heading-row">
        <div>
          <p class="eyebrow">02 / SELECTED WORK</p>
          <h2>Projects I've <span class="gradient-text">worked on.</span></h2>
        </div>
        <p class="heading-description">
          A collection of projects from my learning journey.
        </p>
      </div>

      <div class="projects-grid">
        <!-- Electronics project -->
        <article class="project-card">
          <div class="project-image-wrap">
            <img
                class="project-image"
                src="/images/12v.avif"
                alt="12V electronics project"
            />
          </div>

          <div class="project-content">
            <div class="project-meta">
              <span class="project-category">ELECTRONICS</span>
              <span class="project-status">Learning project</span>
            </div>

            <h3>Electronics Project</h3>
            <p>
              A hands-on electronics project showcasing my interest in
              electronic components, circuits, and practical applications.
            </p>

            <div class="tag-list">
              <span>Electronics</span>
              <span>12V</span>
              <span>Hardware</span>
            </div>
          </div>
        </article>

        <!-- ElectroHub -->
        <article class="project-card">
          <div class="electrohub-visual">
            <div class="electrohub-window">
              <div class="electrohub-top">
                <span class="window-dot"></span>
                <span class="window-dot"></span>
                <span class="window-dot"></span>
                <span class="electrohub-brand">Electro<span>Hub</span></span>
              </div>

              <div class="electrohub-body">
                <span class="electrohub-kicker">COMPONENTS STORE</span>
                <h4>Power your<br />next project.</h4>
                <div class="electrohub-chip">Explore components ↗</div>
                <div class="component-shapes">
                  <span class="component-chip chip-one"></span>
                  <span class="component-chip chip-two"></span>
                  <span class="component-chip chip-three"></span>
                </div>
              </div>
            </div>
          </div>

          <div class="project-content">
            <div class="project-meta">
              <span class="project-category">WEB DEVELOPMENT</span>
              <span class="project-status">In development</span>
            </div>

            <h3>ElectroHub</h3>
            <p>
              A web application concept for browsing electronic components
              with product information, inventory, and pricing.
            </p>

            <div class="tag-list">
              <span>Vue.js</span>
              <span>Django</span>
              <span>API</span>
            </div>
          </div>
        </article>

        <!-- Portfolio -->
        <article class="project-card">
          <div class="portfolio-visual">
            <div class="portfolio-preview">
              <span class="preview-logo">ZM.</span>
              <div class="preview-lines">
                <span></span>
                <span></span>
                <span></span>
              </div>
              <div class="preview-title">My digital<br /><span>space.</span></div>
              <div class="preview-button">Explore my work ↗</div>
              <div class="preview-orb"></div>
            </div>
          </div>

          <div class="project-content">
            <div class="project-meta">
              <span class="project-category">PERSONAL WEBSITE</span>
              <span class="project-status">Live</span>
            </div>

            <h3>Personal Portfolio</h3>
            <p>
              My personal portfolio website built to present my skills,
              projects, and journey as an aspiring developer.
            </p>

            <div class="tag-list">
              <span>Vue.js</span>
              <span>CSS</span>
              <span>Vercel</span>
            </div>

            <div class="project-links">
              <a
                  href="https://zander-portfolio-pxbk5jx3p-electro-hub1.vercel.app"
                  target="_blank"
                  rel="noopener noreferrer"
              >
                Live Website ↗
              </a>
              <a
                  href="https://github.com/zandermamuad6-droid/zander-portfolio"
                  target="_blank"
                  rel="noopener noreferrer"
              >
                GitHub ↗
              </a>
            </div>
          </div>
        </article>
      </div>
    </section>

    <!-- Skills -->
    <section id="skills" class="section-container section-block">
      <div class="section-heading">
        <p class="eyebrow">03 / MY TOOLKIT</p>
        <h2>Skills I'm <span class="gradient-text">developing.</span></h2>
        <p class="section-description">
          These are the technologies and areas I'm learning through practice.
        </p>
      </div>

      <div class="skills-grid">
        <div class="skill-card">
          <span class="skill-symbol">⌘</span>
          <h3>Frontend</h3>
          <p>HTML · CSS · JavaScript · Vue.js</p>
        </div>

        <div class="skill-card">
          <span class="skill-symbol">⌬</span>
          <h3>Backend</h3>
          <p>Python · Django · REST APIs</p>
        </div>

        <div class="skill-card">
          <span class="skill-symbol">▤</span>
          <h3>Tools</h3>
          <p>Git · GitHub · WebStorm · Vercel</p>
        </div>

        <div class="skill-card">
          <span class="skill-symbol">ϟ</span>
          <h3>Electronics</h3>
          <p>Electronic components · Circuits · Hardware</p>
        </div>
      </div>
    </section>

    <!-- Contact -->
    <section id="contact" class="section-container section-block">
      <div class="contact-card">
        <p class="eyebrow">04 / GET IN TOUCH</p>
        <h2>Let's build something <span class="gradient-text">together.</span></h2>
        <p>
          I'm open to learning opportunities, collaborations, and
          conversations about development and technology.
        </p>

        <!-- Palitan ang email address na ito ng sarili mong email. -->
        <a class="button button-primary" href="mailto:your-email@example.com">
          Send Me an Email <span>↗</span>
        </a>
      </div>
    </section>

    <!-- Footer -->
    <footer class="footer section-container">
      <a class="logo" href="#home">ZM.</a>
      <p>Designed and built while learning, one step at a time.</p>
      <p>© 2026 Zander Mamuad</p>
    </footer>
  </main>
</template>
