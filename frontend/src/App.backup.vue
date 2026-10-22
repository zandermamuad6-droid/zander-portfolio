
<script setup>
import { ref } from 'vue'

const menuOpen = ref(false)

const projects = [
  {
    number: '01',
    title: 'Regulated 12V DC Power Supply',
    category: 'Electronics · Engineering',
    description:
        'An electronics project involving AC-to-DC conversion using a transformer, full-wave rectifier, filter capacitor, and LM7812 voltage regulator.',
    tags: ['Electronics', 'Circuit Design', '12V DC'],
  },
  {
    number: '02',
    title: 'Personal Portfolio Website',
    category: 'Web Development · Learning',
    description:
        'This portfolio website, built from scratch while learning Vue.js, CSS, and Django.',
    tags: ['Vue.js', 'CSS', 'Django'],
  },
]

const skills = [
  'Problem Solving',
  'Critical Thinking',
  'Creativity',
  'Circuit Analysis',
  'HTML & CSS — Learning',
  'JavaScript — Learning',
  'Python — Learning',
  'Vue.js — Learning',
  'Django — Learning',
]

const closeMenu = () => {
  menuOpen.value = false
}
</script>

<template>
  <div class="site-shell">
    <header class="navbar">
      <a class="brand" href="#home" @click="closeMenu">ZM<span>.</span></a>

      <button
          class="menu-toggle"
          type="button"
          :aria-expanded="menuOpen"
          aria-label="Toggle navigation"
          @click="menuOpen = !menuOpen"
      >
        {{ menuOpen ? 'Close' : 'Menu' }}
      </button>

      <nav :class="['nav-links', { 'nav-open': menuOpen }]">
        <a href="#about" @click="closeMenu">About</a>
        <a href="#projects" @click="closeMenu">Projects</a>
        <a href="#skills" @click="closeMenu">Skills</a>
        <a class="nav-contact" href="#contact" @click="closeMenu">
          Contact <span>↗</span>
        </a>
      </nav>
    </header>

    <main>
      <section id="home" class="hero section-wrap">
        <div class="hero-copy">
          <div class="availability">
            <span class="status-dot"></span>
            ASPIRING COMPUTER ENGINEER
          </div>

          <h1>
            Hi, I'm Zander.<br />
            I build <span class="gradient-text">my future</span><span class="cursor">.</span>
          </h1>

          <p class="hero-description">
            Exploring technology, engineering, and web development.
            Learning step by step and turning ideas into practical projects.
          </p>

          <div class="hero-actions">
            <a class="button button-primary" href="#projects">
              Explore my work <span>↗</span>
            </a>
            <a class="button button-secondary" href="#contact">
              Get in touch
            </a>
          </div>

          <div class="hero-note">
            <span class="note-line"></span>
            Currently learning web development from the ground up.
          </div>
        </div>

        <div class="hero-visual" aria-label="Decorative technology illustration">
          <div class="orbit orbit-one"></div>
          <div class="orbit orbit-two"></div>
          <div class="orbit orbit-three"></div>
          <div class="orbit-core">
            <span class="core-symbol">&lt;/&gt;</span>
          </div>
          <span class="float-tag tag-top">DESIGN</span>
          <span class="float-tag tag-right">BUILD</span>
          <span class="float-tag tag-bottom">LEARN</span>
          <span class="visual-star star-one">✳</span>
          <span class="visual-star star-two">✦</span>
        </div>

        <a href="#about" class="scroll-cue">
          <span class="scroll-mouse"></span>
          SCROLL TO EXPLORE
        </a>
      </section>

      <section id="about" class="content-section section-wrap">
        <div class="section-heading">
          <span class="eyebrow">01 / ABOUT</span>
          <h2>A little about <span>me.</span></h2>
        </div>

        <div class="about-grid">
          <div class="about-intro">
            <p class="large-copy">
              I'm an aspiring Computer Engineer interested in how technology
              can solve real problems.
            </p>
          </div>

          <div class="about-details">
            <p>
              My interests include systems analysis, problem-solving, and
              building useful technology solutions. I enjoy exploring how
              things work, from electronic circuits to websites.
            </p>
            <p>
              I'm currently starting my web development journey, learning
              the fundamentals and applying them through hands-on projects.
              This portfolio will grow as my skills grow.
            </p>

            <div class="about-facts">
              <div>
                <span class="fact-label">FOCUS</span>
                <span>Engineering & Technology</span>
              </div>
              <div>
                <span class="fact-label">CURRENT GOAL</span>
                <span>Learn and build consistently</span>
              </div>
              <div>
                <span class="fact-label">BASED IN</span>
                <span>Isabela, Philippines</span>
              </div>
            </div>
          </div>
        </div>
      </section>

      <section id="projects" class="content-section section-wrap">
        <div class="section-heading heading-row">
          <div>
            <span class="eyebrow">02 / SELECTED WORK</span>
            <h2>Projects in <span>progress.</span></h2>
          </div>
          <span class="section-count">02 PROJECTS</span>
        </div>

        <div class="project-grid">
          <article
              v-for="project in projects"
              :key="project.number"
              class="project-card"
          >
            <div class="project-top">
              <span class="project-number">{{ project.number }}</span>
              <span class="project-arrow">↗</span>
            </div>

            <div class="project-art" :class="'art-' + project.number">
              <template v-if="project.number === '01'">
                <div class="circuit-board">
                  <span class="circuit-label">AC</span>
                  <span class="circuit-line line-a"></span>
                  <span class="circuit-line line-b"></span>
                  <span class="circuit-chip">12V</span>
                  <span class="circuit-label output-label">DC</span>
                </div>
              </template>
              <template v-else>
                <div class="code-window">
                  <div class="code-window-bar">
                    <i></i><i></i><i></i>
                    <span>portfolio.vue</span>
                  </div>
                  <div class="code-lines">
                    <span class="code-purple">const</span> portfolio = {<br />
                    &nbsp;&nbsp;name: <span class="code-green">'Zander'</span>,<br />
                    &nbsp;&nbsp;learning: <span class="code-green">true</span><br />
                    }
                  </div>
                </div>
              </template>
            </div>

            <span class="project-category">{{ project.category }}</span>
            <h3>{{ project.title }}</h3>
            <p class="project-description">{{ project.description }}</p>

            <div class="project-tags">
              <span v-for="tag in project.tags" :key="tag">{{ tag }}</span>
            </div>
          </article>
        </div>
        <p class="project-disclaimer">
          Project descriptions reflect the information currently available.
          More work and details will be added as projects develop.
        </p>
      </section>

      <section id="skills" class="content-section section-wrap">
        <div class="section-heading">
          <span class="eyebrow">03 / TOOLKIT</span>
          <h2>Skills & <span>learning.</span></h2>
        </div>

        <p class="section-description">
          A starting point. These skills will develop through study,
          practice, and real projects.
        </p>

        <div class="skills-grid">
          <div
              v-for="(skill, index) in skills"
              :key="skill"
              class="skill-item"
          >
            <span class="skill-index">{{ String(index + 1).padStart(2, '0') }}</span>
            <span>{{ skill }}</span>
            <span class="skill-plus">↗</span>
          </div>
        </div>
      </section>

      <section id="contact" class="contact-section section-wrap">
        <span class="eyebrow">04 / CONTACT</span>
        <h2>Let's connect<span class="gradient-text">.</span></h2>
        <p>
          Have a question or want to connect? Feel free to reach out.
        </p>

        <a class="button button-primary" href="mailto:zandermamuad6@gmail.com">
          Email me <span>↗</span>
        </a>

        <div class="contact-meta">
          <span>OPEN TO LEARNING OPPORTUNITIES</span>
          <a href="#home">BACK TO TOP ↑</a>
        </div>
      </section>
    </main>

    <footer class="footer section-wrap">
      <a class="brand" href="#home">ZM<span>.</span></a>
      <p>Designed and built while learning, one step at a time.</p>
      <span>© {{ new Date().getFullYear() }} Zander Mamuad</span>
    </footer>
  </div>
</template>
