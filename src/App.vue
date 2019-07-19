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
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
