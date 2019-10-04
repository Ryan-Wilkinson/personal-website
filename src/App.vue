<template>
  <div id="app">
    <div class="first-section">
      <h1 class="my-name">
        Ryan Wilkinson
      </h1>
      <!-- <ProjectsAccordian /> -->
    </div>
    <div class="second-section">
      <AboutMe />
    </div>
    <div class="third-section">
      Section 3
    </div>
    <div class="fourth-section">
      Section 4
    </div>
  </div>
</template>

<script>
import ProjectsAccordian from './components/ProjectsAccordian'
import AboutMe from './components/AboutMe'

export default {
  name: 'App',
  components: {
    ProjectsAccordian,
    AboutMe,
  },
}
</script>

<style>
body {
  margin: 0;
}
html {
  background-color: black;
  background-size: cover;
  justify-content: center;
  flex-direction: column;
  height: 100vh;
}
.my-name {
  color: white;
  align-self: center;
  font-family: 'avenir';
  font-weight: 100;
  letter-spacing: 0.5em;
  font-size: 4em;
  padding-left: 0.5em;
  text-shadow: -2px 0 black, 0 2px black, 2px 0 black, 0 -2px black;
}
.first-section {
  display: flex;
  background-image: url('../public/images/fire.jpg');
  background-size: cover;
  justify-content: center;
  flex-direction: column;
  height: 100vh;
}
.second-section {
  display: flex;
  background-color: yellow;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  height: 100vh;
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
</style>
