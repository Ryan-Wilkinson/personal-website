<template>
  <div id="app">
    <ProjectsAccordian />
  </div>
</template>

<script>
import ProjectsAccordian from './components/ProjectsAccordian.vue'

export default {
  name: 'app',
  components: {
    ProjectsAccordian
  }
}
</script>

<style>
body {
  display: flex;
  background-image: url('../public/images/fire.jpg');
	background-size: cover;
  background-repeat: no-repeat;
  background-attachment: fixed;
  justify-content: center;
}
</style>
