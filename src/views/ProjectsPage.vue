<template>
  <div class="projects-page">
    <h1>My development work</h1>
    <div class="prev-next-btns">
      <button class="arrow-btn" @click="showDevProject(-1)"><span>← Previous project</span></button>
      <button class="arrow-btn" @click="showDevProject(1)"><span>Next project →</span></button>
    </div>
    <div v-for="project in devProjects" :key="project.title" class="project" :class="{ 'active': currentDevProject==project }">
      <h2>{{ project.title }}</h2>
      <p>{{ project.subtitle }}</p>
      <img :src="project.imagePath" class="project-img" />
    </div>

    <h1>My design work</h1>
    <div class="prev-next-btns">
      <button class="arrow-btn" @click="showDesignProject(-1)"><span>← Previous project</span></button>
      <button class="arrow-btn" @click="showDesignProject(1)"><span>Next project →</span></button>
    </div>
    <div v-for="project in designProjects" :key="project.title" class="project" :class="{ 'active': currentDesignProject==project }">
      <h2>{{ project.title }}</h2>
      <p>{{ project.subtitle }}</p>
      <img :src="project.imagePath" class="project-img" />
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const devProjects = ref([
  {
    title: "Sandbach School Cautions Register",
    subtitle: "behaviour management web application",
    imagePath: "images/dev-project1.png"
  },
  {
    title: "Briefs for Devs",
    subtitle: "project briefs and resources for developers",
    imagePath: "images/dev-project2.png"
  }
]);
const designProjects = ref([
  {
    title: "Bookletz",
    subtitle: "digital booklets and leaflets creation tool",
    imagePath: "images/design-project1.png"
  },
]);

const currentDevProject = ref(devProjects.value[0]);
const currentDesignProject = ref(designProjects.value[0]);

const showDevProject = (increment) => {
  let currentIndex = devProjects.value.indexOf(currentDevProject.value);
  currentIndex = (currentIndex + increment + devProjects.value.length) % devProjects.value.length;
  currentDevProject.value = devProjects.value[currentIndex];
};
const showDesignProject = (increment) => {
  let currentIndex = designProjects.value.indexOf(currentDesignProject.value);
  currentIndex = (currentIndex + increment + designProjects.value.length) % designProjects.value.length;
  currentDesignProject.value = designProjects.value[currentIndex];
};
</script>

<style scoped>
.projects-page {
  margin: 0 3.5rem;
  padding-bottom: 2rem;
}
h1 {
  color: #AFAFAF;
  text-transform: uppercase;
  font-size: 5vw;
  font-weight: 600;
  margin: 3.5rem 0 1rem 0;
}
.prev-next-btns {
  display: flex;
  justify-content: space-between;
}
.arrow-btn {
  background: none;
  border: none;
  padding: 0;
  font: inherit;
  cursor: pointer;
  position: relative;
}
.arrow-btn span {
  position: relative;
  color: white;
  text-decoration: none;
}
.arrow-btn span::after {
  content: '';
  position: absolute;
  width: 100%;
  height: 2px;
  background-color: #FFEF08;
  bottom: -10px;
  left: 0;
  transform: scaleX(1);
  transform-origin: bottom left;
  transition: transform 0.3s ease-out;
}
.arrow-btn:hover span::after {
  transform: scaleX(0);
  transform-origin: bottom right;
}
.project {
  display: none;
  flex-direction: column;
  align-items: center;
  transition: transform 0.3s ease-out;
}

.project.active {
  display: flex;
  transform: translateY(0);
}

.project h2 {
  color: #9E9E9D;
  text-transform: uppercase;
  font-size: 1.8vw;
  font-weight: 500;
  margin: 2rem 0 0.5rem 0;
}
.project p {
  color: #868686;
  margin: 0;
}
.project-img {
  width: 100%;
}

/* Media queries for mobile devices and smaller screens*/
@media only screen and (max-width: 700px) {
  .projects-page {
    margin: 0 2rem;
  }
  h1 {
    font-size: 2.2rem;
    margin: 2rem 0 1.8rem 0;
  }
  .project h2 {
    font-size: 1.4rem;
    margin: 2.7rem 0 0.5rem 0;
    text-align: center;
  }
  .project-img {
    margin: 1.5rem 0;
  }
}
</style>