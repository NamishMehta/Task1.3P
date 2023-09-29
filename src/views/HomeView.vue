<template>
  <section class="portfolio-home">
    <header class="portfolio-header">
      <h1>Namish Mehta</h1>
      <p>Web Developer</p>
    </header>

    <section class="portfolio-intro">
      <p>
        Hello! My Name is Namish and I am a Web Developer with over 2 years of experience. I like creating User Friendly Websites as a hobby.
        Check some of my work below.....
      </p>
    </section>

    <section class="portfolio-projects">
      <h2>My Projects</h2>
      <div class="projects-grid">
        <div class="project-card" v-for="project in projects" :key="project.id">
          <img :src="project.image" :alt="project.name" />
          <h3>{{ project.name }}</h3>
          <p>{{ project.description }}</p>
        </div>
      </div>
    </section>

    <footer class="portfolio-footer">
      <p>
        Thanks For your Visit! Let's
        <a href="mailto:mehtanamish4@icloud.com">Connect</a>.
      </p>
    </footer>
  </section>
</template>

<script setup>
import { ref } from "vue";

import projectImage1 from "../assets/images/profilepic.jpg";

const projects = ref([
  {
    id: 1,
    name: "Project #1",
    description: "This is my First ever Project.",
    image: projectImage1,
  },
  {
    id: 2,
    name: "Project #2",
    description: "I made this recently because I was bored.",
    image: projectImage1,
  },
  {
    id: 3,
    name: "Project #3",
    description: "This one is a creative one I made 4 months ago...",
    image: projectImage1,
  },
]);
</script>

<style scoped>
.portfolio-home {
  font-family: "Arial", sans-serif;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px;
}

.portfolio-header {
  text-align: center;
  margin-bottom: 50px;
}

.portfolio-header h1 {
  font-size: 2.5em;
  margin-bottom: 10px;
}

.portfolio-intro {
  text-align: center;
  margin-bottom: 50px;
}

.portfolio-projects {
  margin-bottom: 50px;
}

.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  gap: 20px;
}

.project-card {
  border: 1px solid #e0e0e0;
  border-radius: 8px;
  overflow: hidden;
}

.project-card img {
  width: 100%;
  height: auto;
}

.project-card h3 {
  text-align: center;
  padding: 10px 0;
}

.portfolio-footer {
  text-align: center;
}
</style>
