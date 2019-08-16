<template>
  <div id="app">
    <Header />
    <ProjectsAccordian />
  </div>
</template>

<script>
import ProjectsAccordian from './components/ProjectsAccordian.vue'
import Header from './components/Header.vue'

export default {
  name: 'app',
  components: {
    ProjectsAccordian,
    Header
  }
}
</script>

<style>
html {
  display: flex;
  background-image: url('../public/images/fire.jpg');
  background-size: cover;
  justify-content: center;
}

body {
  display: flex;
  flex-direction: column; 
  width: 100%;
}

</style>
