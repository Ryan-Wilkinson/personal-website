<template>
  <div id="app">
    <Header id="header" />
    <div class="first-section">
      <h1 class="my-name">
        Ryan Wilkinson
      </h1>
    </div>
    <div class="construction-section construction">
      <Construction />
    </div>
    <!-- <div class="second-section about">
      <About />
    </div>
    <div class="third-section experience">
      <Experience />
    </div>
    <div class="fourth-section projects">
      <ProjectsAccordian />
    </div>
    <div class="fifth-section">
      Section 5
    </div> -->
  </div>
</template>

<script>
import Header from './components/Header'
// import ProjectsAccordian from './components/ProjectsAccordian'
// import About from './components/About'
// import Experience from './components/Experience'
import Construction from './components/Construction'

export default {
  name: 'App',
  components: {
    Header,
    // ProjectsAccordian,
    // About,
    // Experience,
    Construction,
  },
}
</script>

<style scoped>
html {
  background-size: cover;
  justify-content: center;
  flex-direction: column;
  height: 100vh;
}
#header {
  position: absolute;
}
.my-name {
  margin: 0;
  color: white;
  text-align: center;
  font-family: 'avenir';
  font-weight: 100;
  letter-spacing: 0.5em;
  font-size: 4em;
  padding-left: 0.5em;
  text-shadow: -2px 0 black, 0 2px black, 2px 0 black, 0 -2px black;
}
@media only screen and (max-device-width: 1366px) {
  .first-section {
    background-attachment: scroll;
  }
}
.first-section {
  display: flex;
  background-image: url('../public/images/main.jpg');
  background-size: cover;
  background-attachment: fixed;
  justify-content: center;
  flex-direction: column;
  height: 100vh;
  z-index: -1;
}
.construction-section{
  display: flex;
  background-image: url('../public/images/main.jpg');
  background-size: cover;
  background-attachment: fixed;
  justify-content: center;
  flex-direction: column;
  height: 100vh;
  z-index: -1;
}
.second-section {
  display: flex;
  background-color: grey;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  height: 100vh;
  z-index: 1;
}
.third-section {
  background-color: lightblue;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  height: 100vh;
}
.fourth-section {
  background-color: green;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  height: 100vh;
}
.fifth-section {
  background-color: white;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  height: 100vh;
}
</style>
