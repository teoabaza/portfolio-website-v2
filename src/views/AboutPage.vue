<template>
  <div class="about-page">
    <p class="paragraph1"><span>Hi there, I’m Teo.</span> I come from Romania but now live in Sheffield, UK. My journey to becoming a software developer has been unconventional, shaped by diverse experiences and a passion for real-world problem-solving.</p>
    <img src="@/assets/images/girl-coding.png" class="girl-coding-img"/>
    <h1>My story</h1>
    <p class="paragraph2"> I started my professional life studying Translation and Interpretation in English and German. After graduation, life took me on a wild ride. I worked odd jobs in hostels, met incredible people, and explored different corners of the world. Teaching is something I’ve always loved, which is why I became a qualified teacher after completing a PGDE in Sheffield. While I enjoyed mentoring, my heart led me towards coding. I took the self-taught route, learning HTML, CSS, JavaScript and React. In 2022, I landed a gig as a Junior Software Developer at Oasis Studio in Chesterfield, where I dove headfirst into PHP, Vue.js, Laravel, and more. Now, as a freelancer, I'm constantly learning and taking on new challenges in Vue and Laravel.</p>
    <div class="my-approach">
      <h2>My approach</h2>
      <p>I love diving into the heart of problems and finding creative solutions. Working with clients is something I’ve got very good at, because I focus on clear communication and making their ideas a reality (no matter how ridiculous they may sound to a developer!). I work well independently, but thrive in collaborative environments and fully believe in the power of teamwork.</p>
    </div>
    <h1>My life beyond work</h1>
    <div class="my-life-beyond-work">
      <p>When I'm not in front of my computer, you'll find me in the Peaks, walking or climbing. Though if it’s pouring I’ll be reading a nice book or playing boardgames with my friends. I also enjoy expressing my creative side occasionally, through drawing and painting.</p>
      <img src="@/assets/images/teo-climbing.png" class="teo-climbing-img"/>
    </div>
    <p class="paragraph3">If you connect with my work ethic and creative spirit, I'm here, ready to collaborate. Let's turn your ideas into something extraordinary.</p>
    <h1 class="thank-you-heading">Thank you for visiting my portfolio.</h1>
  </div>
</template>

<script setup>


</script>

<style scoped>
.about-page {
  margin: 0 3.5rem;
}
.paragraph1 {
  margin-top: 5rem;
  color: #AFAFAF;
  font-size: 2.1vw;
}
.paragraph1 span {
  color: #FFEF08;
}
.girl-coding-img {
  width: 100%;
}
h1 {
  color: #AFAFAF;
  text-transform: uppercase;
  font-size: 5vw;
  font-weight: 600;
  margin: 3.5rem 0 1rem 0;
}
.paragraph2 {
  color: #AFAFAF;
  font-size: 1.6vw;
  line-height: 1.2;
}
.my-approach {
  background-color: #FFEF08;
  border-radius: 15px;
  color: black;
  padding: 4rem 5rem;
  margin: 4rem 0;
}
.my-approach h2 {
  text-transform: uppercase;
  font-size: 4vw;
  font-weight: 600;
  margin: 0;
}
.my-approach p {
  font-size: 1.7vw;
  margin: 2rem 0 0 0;
}
.my-life-beyond-work {
  margin: 3rem 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.my-life-beyond-work p {
  max-width: 40%;
  font-size: 2vw;
  color: #AFAFAF;
}
.teo-climbing-img {
  max-width: 50%;
}
.paragraph3 {
  font-size: 2.4vw;
}
.thank-you-heading {
  font-size: 5vw;
  color: #ADFF02;
  font-weight: 500;
  padding-bottom: 3.5rem;
}
/* Media queries for mobile devices and smaller screens*/
@media only screen and (max-width: 700px) {
  .about-page {
    margin: 0 2rem;
  }
  h1 {
    font-size: 2.5rem;
    margin: 2rem 0 1rem 0;
  }
  .paragraph1 {
    margin: 2rem 0 1.7rem 0;
    font-size: 0.9rem;
  }
  .paragraph2 {
    font-size: 0.75rem;
  }
  .my-approach {
    padding: 2rem 2.5rem;
    margin: 2.5rem 0;
  }
  .my-approach h2 {
    font-size: 1.9rem;
  }
  .my-approach p {
    font-size: 0.7rem;
    margin: 1.2rem 0 0 0;
  }
  .my-life-beyond-work {
    margin: 2rem 0;
    flex-direction: column-reverse;
    justify-content: center;
  }
  .my-life-beyond-work p {
    max-width: unset;
    font-size: 0.9rem;
    margin: 1rem 0 0 0;
  }
  .teo-climbing-img {
    width: 100%;
    max-width: unset;
  }
  .paragraph3 {
    margin-top: 2.5rem;
    font-size: 1rem;
  }
  .thank-you-heading {
    font-size: 2.7rem;
    padding-bottom: 2rem;
  }
}
</style>
