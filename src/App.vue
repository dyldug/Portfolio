<script setup>
const skills = [
  'Linux & Bash',
  'Docker & Kubernetes',
  'Terraform',
  'AWS & Azure',
  'GitHub Actions & GitLab CI',
  'Prometheus & Grafana',
]
</script>

<template>
  <main class="container">
    <section class="hero">
      <p class="eyebrow">DevOps Engineer</p>
      <h1>Dylan Dugadko</h1>
      <p class="intro">
        I build reliable infrastructure, automate delivery pipelines,
        and enjoy making systems easier to operate.
      </p>
      <a href="https://github.com/dyldug" target="_blank" rel="noreferrer">
        View GitHub
      </a>
    </section>

    <section>
      <h2>Skills</h2>
      <ul class="skills">
        <li v-for="skill in skills" :key="skill">{{ skill }}</li>
      </ul>
    </section>

    <section>
      <h2>Projects</h2>
      <article class="project">
        <h3>Coming soon</h3>
        <p>My DevOps projects will live here.</p>
      </article>
    </section>
  </main>
</template>