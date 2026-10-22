<template>
  <div class="portfolio">
    <!-- HEADER -->
    <header class="site-header">
      <div class="container nav-container">
        <a class="logo" href="#home">ZM<span>.</span></a>
        <nav class="navigation">
          <a href="#home">Home</a>
          <a href="#about">About</a>
          <a href="#projects">Projects</a>
          <a href="#skills">Skills</a>
          <a href="#contact">Contact</a>
        </nav>
        <a class="nav-cta" href="#contact">Let's Talk <span>↗</span></a>
      </div>
    </header>

    <main>
      <!-- HERO -->
      <section id="home" class="hero-section">
        <div class="container hero-grid">
          <div class="hero-content">
            <div class="availability">
              <span class="status-dot"></span>
              Aspiring Developer · Open to Opportunities
            </div>
            <p class="eyebrow">HELLO, I'M</p>
            <h1>Zander<br /><span class="gradient-text">Mamuad.</span></h1>
            <h2>Future Software Developer</h2>
            <p class="hero-description">
              I'm building my skills in web development, programming, and
              electronics. I enjoy learning how things work and turning ideas
              into useful projects.
            </p>
            <div class="hero-buttons">
              <a class="button button-primary" href="#projects">
                Explore My Work <span>↗</span>
              </a>
              <a class="button button-secondary" href="#about">More About Me</a>
            </div>
            <div class="hero-stats">
              <div><strong>01<span>+</span></strong><small>Projects in Progress</small></div>
              <div><strong>03<span>+</span></strong><small>Areas of Interest</small></div>
              <div><strong>∞</strong><small>Things to Learn</small></div>
            </div>
          </div>

          <div class="hero-visual">
            <div class="visual-glow"></div>
            <div class="code-window">
              <div class="window-top">
                <div class="window-dots"><span></span><span></span><span></span></div>
                <span class="window-title">developer.js</span>
                <span class="window-menu">•••</span>
              </div>
              <div class="code-content">
                <p class="code-line"><span class="line-number">01</span> <span class="code-purple">const</span> <span class="code-blue">developer</span> = {</p>
                <p class="code-line indent"><span class="code-blue">name</span>: <span class="code-green">'Zander Mamuad'</span>,</p>
                <p class="code-line indent"><span class="code-blue">role</span>: <span class="code-green">'Student Developer'</span>,</p>
                <p class="code-line indent"><span class="code-blue">interests</span>: [</p>
                <p class="code-line indent-more"><span class="code-green">'Web Development'</span>,</p>
                <p class="code-line indent-more"><span class="code-green">'Electronics'</span>,</p>
                <p class="code-line indent-more"><span class="code-green">'Technology'</span></p>
                <p class="code-line indent">],</p>
                <p class="code-line indent"><span class="code-blue">mindset</span>: <span class="code-green">'Always Learning'</span></p>
                <p class="code-line">};</p>
                <p class="code-line code-comment">// Building something better every day.</p>
              </div>
              <div class="code-footer">
                <span><span class="status-dot"></span> Always learning</span>
                <span>UTF-8</span>
              </div>
            </div>
            <div class="floating-card floating-card-top">
              <span class="floating-icon">⌘</span>
              <div><strong>Creative Thinking</strong><small>Ideas into reality</small></div>
            </div>
            <div class="floating-card floating-card-bottom">
              <span class="floating-icon purple-icon">✦</span>
              <div><strong>Continuous Growth</strong><small>One step at a time</small></div>
            </div>
          </div>
        </div>
        <a href="#about" class="scroll-indicator"><span></span> SCROLL TO EXPLORE</a>
      </section>

      <!-- ABOUT -->
      <section id="about" class="section-container section-block">
        <div class="section-heading">
          <p class="eyebrow">GET TO KNOW ME</p>
          <h2>About <span class="gradient-text">Me</span></h2>
          <p>A little about who I am and what I'm working toward.</p>
        </div>
        <div class="about-grid">
          <div class="about-card about-main-card">
            <div class="card-symbol">✳</div>
            <h3>A learner with a passion for technology.</h3>
            <p>
              I'm an aspiring developer interested in creating websites,
              understanding software, and exploring electronics. I'm currently
              focused on strengthening my fundamentals and gaining practical
              experience through personal projects.
            </p>
            <p>I believe progress comes from consistency, curiosity, and the willingness to learn from mistakes.</p>
          </div>
          <div class="about-side">
            <div class="about-card mini-card">
              <span class="mini-card-icon">⌘</span>
              <div><h3>Development</h3><p>Learning to build useful digital experiences.</p></div>
            </div>
            <div class="about-card mini-card">
              <span class="mini-card-icon">ϟ</span>
              <div><h3>Electronics</h3><p>Exploring circuits and electronic components.</p></div>
            </div>
            <div class="about-card mini-card">
              <span class="mini-card-icon">↗</span>
              <div><h3>Personal Growth</h3><p>Improving my skills one day at a time.</p></div>
            </div>
          </div>
        </div>
      </section>

      <!-- PROJECTS -->
      <section id="projects" class="section-container section-block">
        <div class="section-heading">
          <p class="eyebrow">WHAT I'VE BEEN WORKING ON</p>
          <h2>Featured <span class="gradient-text">Projects</span></h2>
          <p>Projects that reflect my learning journey and interests.</p>
        </div>
        <div class="projects-grid">
          <article class="project-card">
            <div class="project-image-wrap">
              <img
                  class="project-image"
                  src="/images/12v.avif"
                  alt="12V electronics project"
                  loading="eager"
                  @error="imageError = true"
                  @load="imageError = false"
              />
              <div v-if="imageError" class="image-fallback">
                <span class="fallback-icon">ϟ</span>
                <p>Electronics Project</p>
                <small>Check public/images/12v.avif</small>
              </div>
              <span class="image-label">PROJECT 01</span>
            </div>
            <div class="project-content">
              <div class="project-meta">
                <span class="project-category">ELECTRONICS</span>
                <span class="project-status"><span class="status-dot"></span> Learning project</span>
              </div>
              <h3>Electronics Project</h3>
              <p>A hands-on electronics project showcasing my interest in electronic components, circuits, and practical applications.</p>
              <div class="tag-list"><span>Electronics</span><span>12V</span><span>Hardware</span></div>
            </div>
          </article>

          <article class="project-card">
            <div class="electrohub-visual">
              <div class="circuit-decoration circuit-one"></div>
              <div class="circuit-decoration circuit-two"></div>
              <div class="electrohub-mark">
                <span class="electrohub-symbol">ϟ</span>
                <span class="electrohub-name">Electro<span>Hub</span></span>
                <small>COMPONENT MANAGEMENT</small>
              </div>
              <span class="image-label">PROJECT 02</span>
            </div>
            <div class="project-content">
              <div class="project-meta">
                <span class="project-category">WEB APPLICATION</span>
                <span class="project-status"><span class="status-dot"></span> In development</span>
              </div>
              <h3>ElectroHub</h3>
              <p>A component management application concept designed to help organize electronic components, quantities, and prices.</p>
              <div class="tag-list"><span>Vue.js</span><span>Python</span><span>Django</span></div>
            </div>
          </article>

          <article class="project-card">
            <div class="portfolio-visual">
              <div class="portfolio-browser">
                <div class="browser-bar"><span></span><span></span><span></span></div>
                <div class="browser-body">
                  <div class="browser-sidebar"></div>
                  <div class="browser-lines"><span></span><span></span><span></span><div class="browser-block"></div></div>
                </div>
              </div>
              <span class="image-label">PROJECT 03</span>
            </div>
            <div class="project-content">
              <div class="project-meta">
                <span class="project-category">WEB DEVELOPMENT</span>
                <span class="project-status"><span class="status-dot"></span> Live website</span>
              </div>
              <h3>Personal Portfolio</h3>
              <p>My personal portfolio website, built to showcase my projects, technical interests, and progress as a developer.</p>
              <div class="tag-list"><span>Vue.js</span><span>CSS</span><span>Vite</span></div>
              <div class="project-links">
                <a href="https://zander-portfolio-neon.vercel.app" target="_blank" rel="noopener noreferrer">Live Website <span>↗</span></a>
                <a href="https://github.com/zandermamuad6-droid/zander-portfolio" target="_blank" rel="noopener noreferrer">GitHub <span>↗</span></a>
              </div>
            </div>
          </article>
        </div>
      </section>

      <!-- SKILLS -->
      <section id="skills" class="section-container section-block">
        <div class="section-heading">
          <p class="eyebrow">MY CURRENT TOOLKIT</p>
          <h2>Skills &amp; <span class="gradient-text">Technologies</span></h2>
          <p>Tools and topics I'm learning and practicing.</p>
        </div>
        <div class="skills-grid">
          <div class="skill-card">
            <span class="skill-icon">⌘</span><h3>Frontend</h3><p>Building the visual side of websites.</p>
            <div class="tag-list"><span>HTML</span><span>CSS</span><span>JavaScript</span><span>Vue.js</span></div>
          </div>
          <div class="skill-card">
            <span class="skill-icon">⚙</span><h3>Backend</h3><p>Learning application logic and APIs.</p>
            <div class="tag-list"><span>Python</span><span>Django</span><span>REST API</span></div>
          </div>
          <div class="skill-card">
            <span class="skill-icon">ϟ</span><h3>Electronics</h3><p>Exploring hardware and circuit fundamentals.</p>
            <div class="tag-list"><span>Components</span><span>Circuits</span><span>12V Systems</span></div>
          </div>
          <div class="skill-card">
            <span class="skill-icon">⌘</span><h3>Tools</h3><p>Tools that support my development workflow.</p>
            <div class="tag-list"><span>Git</span><span>GitHub</span><span>WebStorm</span><span>Vite</span></div>
          </div>
        </div>
        <p class="skills-note">I'm continuously learning. These skills represent my current areas of study and practice.</p>
      </section>

      <!-- CONTACT -->
      <section id="contact" class="section-container section-block">
        <div class="contact-card">
          <div class="contact-decoration"></div>
          <p class="eyebrow">HAVE A PROJECT IN MIND?</p>
          <h2>Let's build something <span class="gradient-text">great.</span></h2>
          <p>I'm always interested in learning, collaborating, and connecting with people who share a passion for technology.</p>
          <a
              class="button button-primary"
              href="https://mail.google.com/mail/?view=cm&fs=1&to=zandermamuad6@gmail.com"
              target="_blank"
              rel="noopener noreferrer"
          >
            Get In Touch <span>↗</span>
          </a>
          <small class="email-note">Click the button above to compose an email to me.</small>
        </div>
      </section>
    </main>

    <!-- FOOTER -->
    <footer class="site-footer">
      <div class="container footer-content">
        <a class="logo" href="#home">ZM<span>.</span></a>
        <p>Designed and built with curiosity.</p>
        <span>© {{ currentYear }} Zander Mamuad</span>
      </div>
    </footer>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const currentYear = new Date().getFullYear()
const imageError = ref(false)
</script>
