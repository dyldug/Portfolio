<script setup>
const skills = [
  'Linux & Bash',
  'Docker & Kubernetes',
  'Terraform',
  'AWS & Azure',
  'GitHub Actions & GitLab CI',
  'Prometheus & Grafana',
]
const projects = [
  {
    title: 'Dockerized Monitoring Stack',
    description: 'A local Prometheus and Grafana stack for monitoring containerized services.',
    stack: ['Docker', 'Prometheus', 'Grafana'],
    url: 'https://github.com/dyldug',
  },
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
      <article v-for="project in projects" :key="project.title" class="project">
        <h3>{{ project.title }}</h3>
        <p>{{ project.description }}</p>

        <p class="stack">{{ project.stack.join(' · ') }}</p>

        <a :href="project.url" target="_blank" rel="noreferrer">
          View project
        </a>
      </article>
    </section>
  </main>
</template>