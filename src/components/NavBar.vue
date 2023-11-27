<template>
  <div class="navbar">
    <ul class="navbar-items">
      <li :class="{ 'active': currentRoute == '/home' || currentRoute == '/' }"><a href="/home">Home</a></li>
      <li :class="{ 'active': currentRoute == '/about' }"><a href="/about">About me</a></li>
      <li :class="{ 'active': currentRoute == '/projects' }"><a href="/projects">Projects</a></li>
      <li :class="{ 'active': currentRoute == '/contact' }"><a @click="handleContactClick">Contact</a></li>
    </ul>
  </div>
</template>

<script setup>
import { ref, onMounted, watch } from 'vue';
import router from '../router';

const currentRoute = ref(window.location.pathname);

onMounted(() => {
  window.addEventListener('popstate', () => {
    currentRoute.value = window.location.pathname;
  });
});

watch(currentRoute, (newValue, oldValue)=>{
  if(newValue && newValue!=oldValue && newValue!='/home'){
    document.getElementById('job-title').style.display = 'none';
  }
});

function handleContactClick() {
  router.push('/home').then(() => {
    setTimeout(() => {
      const contactSection = document.getElementById('contact');
      if (contactSection) {
        contactSection.scrollIntoView({ behavior: 'smooth' });
      }
    }, 100);
  });
}
</script>

<style scoped>
.navbar {
  display: flex;
  justify-content: flex-end;
  margin: 2rem 3rem;
}
.navbar-items {
  display: flex;
  margin: 0;
}
.navbar-items li {
  /* font-family: 'Varta', Arial, Helvetica, sans-serif; */
  font-weight: 300;
  list-style-type: none;
  text-align: right;
  margin-left: 2rem;
  color: #AFAFAF;
}
.navbar-items a {
  text-decoration: none;
  color: inherit;
  cursor: pointer;
}
.navbar-items a:hover {
  color: white;
}
.active {
  color: white !important;
}
/* Media queries for mobile devices and smaller screens*/
@media only screen and (max-width: 700px) {
  .navbar {
    justify-content: center;
    margin: 2rem 1rem 1rem 1rem;
  }
  .navbar-items {
    width: 100%;
    justify-content: space-between;
    padding: 0;
  }
  .navbar-items li {
    font-size: 0.8rem;
    margin-left: 1rem;
  }
}
</style>