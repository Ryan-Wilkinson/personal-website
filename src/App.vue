<template>
  <div id="app">
    <div class="first-container">
      <Header />
      <ProjectsAccordian />
    </div>
  </div>
</template>

<script>
import ProjectsAccordian from './components/ProjectsAccordian.vue'
import Header from './components/Header.vue'

export default {
  name: 'App',
  components: {
    ProjectsAccordian,
    Header
  }
}
</script>

<style>
.first-container {
  display: flex;
  background-image: url('../public/images/fire.jpg');
  background-size: cover;
  justify-content: center;
  flex-direction: column;
}

</style>
