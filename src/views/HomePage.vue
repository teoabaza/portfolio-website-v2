<template>
  <div class="home-page">
    <!-- hello intro and photo section -->
    <div id="intro">
      <div class="intro-text">
        <h1>Hello World!</h1>
        <h1>I'm a full stack web developer based in Sheffield, UK.</h1>
        <p class="subtitle">Hi, my name is Teo. I’m a full stack developer and I also enjoy UI/UX design. I work with JavaScript and PHP. Check out <a href="/projects">my portfolio</a> and <a href="#contact">contact me</a>.</p>
        <div class="intro-btns">
          <button id="contact-me-btn" @click="scrollToContact">Contact me</button>
          <button id="portfolio-btn" @click="router.push('/projects')">My portfolio</button>
        </div>
      </div>
      <img src="@/assets/images/TeoAbaza.png" class="teo-banner-img"/>
    </div>
    <!-- experience in numbers section -->
    <div id="experience-in-numbers">
      <div class="exp-box"><div class="exp-nr">4</div><div class="exp-text">Web applications built</div></div>
      <div class="exp-box"><div class="exp-nr">9</div><div class="exp-text">Web designs created</div></div>
      <div class="exp-box"><div class="exp-nr">1.5</div><div class="exp-text">Years experience</div></div>
    </div>
    <!-- short about me description -->
    <p id="short-about">
      I specialise in transforming ideas into user-friendly software. With a passion for problem-solving and an eye for clean design, I create innovative solutions that prioritise a seamless user experience. Explore my portfolio to see how I turn concepts into intuitive web applications. 
    </p>
    <!-- services description -->
    <div id="services">
      <div class="service-desc" id="service-desc1">
        <h1>UI/UX Design</h1>
        <p>When designing bespoke applications, my process involves researching the target audience and the competitors. I usually create multiple designs and fully workng prototypes in Figma, so clients can choose the closest representation to their vision.</p>
      </div>
      <div class="service-desc">
        <h1>Software Development</h1>
        <p>I create most web applications using Vue.js and Laravel, although I have also dabbled with React and Express. I have built several websites and web applications from scratch, ranging from static websites to complex platforms.</p>
      </div>
    </div>
    <!-- projects section -->
    <div id="projects">
      <h1>My recent projects</h1>
      <div class="project1">
        <img src="@/assets/images/home-project1.png" id="proj-img-1" class="project-showcase-img parallax-img"/>
        <div class="project1-details">
          <h2>Sandbach School Cautions Register</h2>
          <h3>Design / Development</h3>
          <p>behaviour management web application</p>
          <button class="learn-more-btn" @click="router.push('/project1')"><span>Read more →</span></button>
        </div>
      </div>
      <div class="project2">
        <img src="@/assets/images/home-project2.png" id="proj-img-2" class="project-showcase-img parallax-img"/>
        <div class="project2-details">
          <h2>Bookletz</h2>
          <h3>UI/UX Design</h3>
          <p>digital booklets and leaflets creation tool</p>
          <button class="learn-more-btn" @click="router.push('/project2')"><span>Read more →</span></button>
        </div>
      </div>
    </div>
    <!-- skills section -->
    <div id="skills">
      <h1>My tech stack</h1>
      <div class="skills-boxes">
        <div class="flip-box">
          <div class="flip-box-inner">
            <div class="flip-box-front">
              <img src="@/assets/icons/html5.png" class="skill"/>
            </div>
            <div class="flip-box-back">
                <p class="flip-box-back-text">HTML 5</p>
            </div>
          </div>
        </div>
        <div class="flip-box">
          <div class="flip-box-inner">
            <div class="flip-box-front">
              <img src="@/assets/icons/css3.png" class="skill"/>
            </div>
            <div class="flip-box-back">
                <p class="flip-box-back-text">CSS 3</p>
            </div>
          </div>
        </div>
        <div class="flip-box">
          <div class="flip-box-inner">
            <div class="flip-box-front">
              <img src="@/assets/icons/javascript.png" class="skill"/>
            </div>
            <div class="flip-box-back">
                <p class="flip-box-back-text">JavaScript</p>
            </div>
          </div>
        </div>
        <div class="flip-box">
          <div class="flip-box-inner">
            <div class="flip-box-front">
              <img src="@/assets/icons/php.png" class="skill"/>
            </div>
            <div class="flip-box-back">
                <p class="flip-box-back-text">PHP</p>
            </div>
          </div>
        </div>
        <div class="flip-box">
          <div class="flip-box-inner">
            <div class="flip-box-front">
              <img src="@/assets/icons/vue.png" class="skill"/>
            </div>
            <div class="flip-box-back">
                <p class="flip-box-back-text">Vue Js</p>
            </div>
          </div>
        </div>
        <div class="flip-box">
          <div class="flip-box-inner">
            <div class="flip-box-front">
              <img src="@/assets/icons/laravel.png" class="skill"/>
            </div>
            <div class="flip-box-back">
                <p class="flip-box-back-text">Laravel</p>
            </div>
          </div>
        </div>
        <div class="flip-box">
          <div class="flip-box-inner">
            <div class="flip-box-front">
              <img src="@/assets/icons/git.png" class="skill"/>
            </div>
            <div class="flip-box-back">
                <p class="flip-box-back-text">Git</p>
            </div>
          </div>
        </div>
        <div class="flip-box">
          <div class="flip-box-inner">
            <div class="flip-box-front">
              <img src="@/assets/icons/azure-devops.png" class="skill"/>
            </div>
            <div class="flip-box-back">
                <p class="flip-box-back-text">Azure DevOps</p>
            </div>
          </div>
        </div>
        <div class="flip-box">
          <div class="flip-box-inner">
            <div class="flip-box-front">
              <img src="@/assets/icons/figma.png" class="skill"/>
            </div>
            <div class="flip-box-back">
                <p class="flip-box-back-text">Figma</p>
            </div>
          </div>
        </div>
        <div class="flip-box">
          <div class="flip-box-inner">
            <div class="flip-box-front">
              <img src="@/assets/icons/adobe-illustrator.png" class="skill"/>
            </div>
            <div class="flip-box-back">
                <p class="flip-box-back-text">Adobe Illustrator</p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- contact section -->
    <div id="contact">
      <h1>Get in touch with me</h1>
      <div class="contact-inputs-container">
        <input type="text" class="name-input" placeholder="name..." v-model="emailParams.sender_name"/>
        <input type="email" class="email-input" placeholder="email..." v-model="emailParams.sender_email"/>
        <textarea placeholder="message..." class="message-input" v-model="emailParams.sender_message"></textarea>
        <div class="send-btn-container"><button @click="sendEmail">send</button></div>
      </div>
    </div>

    <div class="social-icons-container">
      <a href="https://www.linkedin.com/in/teodoraabaza/" target="_blank"><img src="@/assets/icons/linkedin.png" class="social-icon"/></a>
      <a href="https://github.com/teoabaza" target="_blank"><img src="@/assets/icons/github.png" class="social-icon"/></a>
      <a href="mailto:teodoraabaza@gmail.com" target="_blank"><img src="@/assets/icons/mail.png" class="social-icon"/></a>
    </div>

    <p class="designed-by">2023 | Designed by Teo with ♡</p>
    
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue';
import router from '../router';
import emailjs from '@emailjs/browser';
import { loading, notify } from '../hooks/globals';

const projectImages = ref([]);
let scrollValue = 0;

onMounted(() => {
  projectImages.value = document.querySelectorAll('.project-showcase-img');
  window.addEventListener('scroll', handleScroll);
});

function scrollToContact() {
  const contactSection = document.getElementById('contact');
  if (contactSection) {
    contactSection.scrollIntoView({ behavior: 'smooth' });
  }
}

function handleScroll() {
  scrollValue = window.scrollY;
  requestAnimationFrame(moveImages);
}

function moveImages() {
  const windowHeight = window.innerHeight;
  projectImages.value.forEach((image) => {
    const rect = image.getBoundingClientRect();
    const translateY = ((rect.top + rect.height / 2 - windowHeight / 2) * 0.1);
    image.style.transform = `translateY(${translateY}px)`;
  });
}


//email parameters
const emailParams = ref({
  sender_name: '',
  sender_email: '',
  sender_message: '',
});

function sendEmail(){
  if (emailParams.value.sender_name && emailParams.value.sender_email && emailParams.value.sender_message) {
    loading.value = true;
    emailjs.send("contact_service", "contact_form", emailParams.value, "9ZP3HD_LR2dZqLN7k")
    .then((response) => {
      console.log('Message sent successfully:', response);
      notify('SENT','Message sent successfuly','#5EBB8D',2000);
      // Reset form fields after successful submission
      emailParams.value.sender_name = '';
      emailParams.value.sender_email = '';
      emailParams.value.sender_ = '';
      loading.value = false;
    })
    .catch((e) => {
      alert("Sorry. Something went wrong. Email not sent.");
      console.log(e);
      loading.value = false;
    });
  } else alert('Please fill out all fields.');
}

</script>

<style scoped>
.home-page {
  margin: 0 3.5rem;
}
.teo-banner-img {
  max-width: 26vw;
}
#intro {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 2.5rem 0 4.5rem 0;
}
.intro-text {
  max-width: 45vw;
}
.intro-text h1 {
  font-size: 4.2vw;
  text-transform: uppercase;
  font-weight: normal;
  margin: 0;
}
.subtitle {
  font-size: 1.7vw;
  color: #AFAFAF;
}
.subtitle a {
  text-decoration: none;
  color: #FFEF08;
}
.subtitle a:hover {
  color: #F94548;
}
.intro-btns {
  margin: 2rem 0;
}
.intro-btns button {
  background-color: #FFEF08;
  border: 2px solid #FFEF08;
  font-family: 'Urbanist', Arial, Helvetica, sans-serif;
  font-weight: 600;
  border-radius: 10px;
  padding: 1rem 2rem;
  margin-right: 1rem;
  box-shadow: rgba(0, 0, 0, 0.19) 0px 10px 20px, rgba(0, 0, 0, 0.23) 0px 6px 6px;
  cursor: pointer;
  transition: transform 0.2s ease-in-out;
}
.intro-btns button:hover {
  transform: translateY(-5px);
}
#portfolio-btn {
  background-color: transparent;
  color: #E1E1E1;
  border: 2px solid #E1E1E1;
}
#experience-in-numbers {
  background-color: white;
  border-radius: 15px;
  display: flex;
  justify-content: space-evenly;
}
.exp-box {
  display: flex;
  align-items: center;
  justify-content: center;
  color: black;
  padding: 2rem;
  max-width: 160px;
}
.exp-nr {
  font-size: 8vw;
  font-weight: 600;
  margin-right: 1rem;
}
.exp-text {
  font-size: 2vw;
  font-weight: 500;
}
#short-about {
  color: #AFAFAF;
  font-size: 2.6vw;
  padding: 2.8rem 0;
}
#services {
  background-color: #F94548;
  border-radius: 15px;
  color: black;
  padding: 4rem 5rem;
}
.service-desc h1 {
  text-transform: uppercase;
  font-size: 4vw;
  font-weight: 600;
  margin: 0;
}
.service-desc p {
  font-size: 1.7vw;
}
#service-desc1 {
  margin-bottom: 3rem;
}
#projects {
  padding: 6rem 0 2rem 0;
}
#projects h1 {
  color: #AFAFAF;
  text-transform: uppercase;
  font-size: 5vw;
  font-weight: 600;
  margin: 0 0 1rem 0;
}
#projects h2 {
  color: #9E9E9D;
  text-transform: uppercase;
  font-size: 2.5vw;
  font-weight: 500;
  margin: 1rem 0;
}
#projects h3 {
  text-transform: capitalize;
  font-weight: 500;
  margin: 0;
}
#projects p {
  color: #868686;
  margin: 2rem 0 2.5rem 0;
  max-width: 250px;
}
.project-showcase-img {
  max-width: 60vw;
  border: 1rem solid black;
  border-radius: 15px;
}
#proj-img-2 {
  border: 1rem solid #AFAFAF;
}
.project1, .project2 {
  display: flex;
  padding: 1rem 0 2rem 0;
}
.project2 {
  flex-direction: row-reverse;
}
.project1-details {
  margin-left: 2rem;
}
.project2-details {
  margin-right: 2rem;
}
.learn-more-btn {
  background: none;
  border: none;
  padding: 0;
  font: inherit;
  cursor: pointer;
  position: relative;
}
.learn-more-btn span {
  position: relative;
  color: white;
  text-decoration: none;
}
.learn-more-btn span::after {
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
.learn-more-btn:hover span::after {
  transform: scaleX(0);
  transform-origin: bottom right;
}
#skills {
  margin: 0 0 6rem 0;
}
#skills h1 {
  color: #AFAFAF;
  text-transform: uppercase;
  font-size: 5vw;
  font-weight: 600;
  margin: 0 0 1.5rem 0;
}
.skills-boxes {
  width: calc(100% - 4rem);
  background-color: #F94548;
  border-radius: 15px;
  display: inline-flex;
  justify-content: center;
  flex-wrap: wrap;
  padding: 3rem 2rem;
}
.flip-box {
  width: 8vw;
  height: 8vw;
  margin: 0.5rem 0.1rem;
}
.flip-box-inner {
  position: relative;
  width: 100%;
  height: 100%;
  text-align: center;
  transition: transform 0.8s;
  transform-style: preserve-3d;
}
.flip-box:hover .flip-box-inner {
  transform: rotateY(180deg);
}
.flip-box-front, .flip-box-back {
  position: absolute;
  width: 100%;
  height: 100%;
  -webkit-backface-visibility: hidden;
  backface-visibility: hidden;
}
.flip-box-back {
  transform: rotateY(180deg);
  border: solid 3.2px;
  border-color: #000000;
  color: rgb(0, 0, 0);
  text-align: center;
  display: flex;
  justify-content: center;
  align-items: center;
}
.flip-box-back-text {
  font-weight: bold;
  font-size: 1.5vw;
}
.skill {
  width: 90%;
}
#contact {
  background-color: #FFEF08;
  border-radius: 15px;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  padding: 6vw 2vw;
}
#contact h1 {
  color: black;
  font-size: 5vw;
  text-transform: uppercase;
  max-width: 30%;
}
.contact-inputs-container {
  width: 50%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.name-input, .email-input, .message-input {
  width: 60%;
  background-color: transparent;
  border: 3px solid black;
  border-radius: 5px;
  padding: 8px 15px;
}
.email-input, .name-input {
  margin-bottom: 0.8rem;
}
.email-input, .name-input, .message-input {
  color: #F94548;
}
.email-input:focus, .name-input:focus, .message-input:focus {
  outline: none;
  border: 3px solid #F94548;
}
.name-input::placeholder, .email-input::placeholder, .message-input::placeholder {
  font-size: 0.75rem;
  font-weight: 300;
  color: black;
}
.message-input {
  min-height: 100px;
}
.send-btn-container {
  display: flex;
  justify-content: center;
  margin-top: 2rem;
}
.send-btn-container button {
  font-size: 1.5vw;
  font-weight: 600;
  text-transform: uppercase;
  border-radius: 10px;
  background-color: white;
  color: black;
  border: 2px solid black;
  padding: 1rem 2.5rem;
  font-family: 'Urbanist', Arial, Helvetica, sans-serif;
  cursor: pointer;
}
.send-btn-container button:hover {
  background-color: #F94548;
}
.social-icons-container {
  width: 100%;
  margin: 4rem 0 2rem 0;
  display: flex;
  justify-content: center;
}
.social-icon {
  width: 5vw;
  margin: 0 1rem 0 1rem;
  animation: hover-effect 3s infinite;
}
.social-icon:hover {
  opacity: 0.6;
}
.parallax-img {
  transition: transform 0.3s ease-out;
}
.designed-by {
  width: 100%;
  text-align:center;
  color: #868686;
  font-size: 1.5vw;
  font-weight: 300;
  padding:  0 0 3.5rem 0;
}

/* Media queries for mobile devices and smaller screens*/
@media only screen and (max-width: 700px) {
  .home-page {
    margin: 0 2rem;
  }
  #intro {
    flex-direction: column-reverse;
    padding: 1.5rem 0 0 0;
  }
  .teo-banner-img {
    width: 100%;
    max-width: unset;
  }
  .intro-text {
    max-width: unset;
    margin: 1.5rem 0 0.8rem 0;
  }
  .intro-text h1 {
    font-size: 1.7rem;
  }
  .subtitle {
    font-size: 0.8rem;
  }
  #experience-in-numbers {
    width: fit-content;
    flex-direction: column;
    align-items: center;
  }
  .exp-box {
    padding: 1.5rem 2.5rem;
  }
  .exp-text {
    font-size: 1rem;
  }
  #short-about {
    font-size: 1.2rem;
    padding: 1.5rem 0;
  }
  #services {
    padding: 2rem 3rem;
  }
  .service-desc h1 {
    font-size: 2rem;
  }
  .service-desc p {
    font-size: 0.8rem;
  }
  #service-desc1 {
    margin-bottom: 1.7rem;
  }
  #projects {
    padding: 3rem 0 1rem 0;
  }
  #projects h1 {
    font-size: 2.7rem;
  }
  #projects h2 {
    font-size: 1.2rem;
  }
  #projects p {
    margin: 1rem 0 2rem 0;
    font-size: 0.8rem;
  }
  .project-showcase-img {
    max-width: unset;
    margin: 3rem 0 1rem 0;
  }
  .project1, .project2 {
    padding: 1rem 0 0 0;
    flex-direction:column-reverse;
  }
  .project1-details {
    margin-left: 0;
  }
  #skills {
    margin: 0 0 3.5rem 0;
  }
  #skills h1 {
    font-size: 2.7rem;
  }
  .skills-boxes {
    width: calc(100% - 2rem);
    padding: 2rem 1rem;
  }
  .flip-box {
    width: 4rem;
    height: 4rem;
  }
  .flip-box-back-text {
    font-size: 0.8rem;
  }
  #contact {
    padding: 2rem;
    flex-direction: column;
  }
  #contact h1 {
    font-size: 2.2rem;
    max-width: unset;
  }
  .contact-inputs-container {
    width: 100%;
  }
  .send-btn-container button {
    font-size: 1rem;
  }
  .name-input, .email-input, .message-input {
    width: 80%;
  }
  .social-icon {
    width: 3.5rem;
  }
  .designed-by {
    font-size: 0.7rem;
    padding: 0 0 1rem 0;
  }
}
</style>
