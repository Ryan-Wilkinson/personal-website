<template>
  <div class="main-header-wrapper">
    <img
      class="header-icon"
    >
    <div class="nav-button-wrapper">
      <div
        href="#"
        @click="scrollToAbout"
      >
        About
      </div>
      <div
        href="#"
        @click="scrollToExperience"
      >
        Experience
      </div>
      <div
        href="#"
        @click="scrollToProjects"
      >
        Projects
      </div>
      <div
        href="#"
        @click="scrollToTBD"
      >
        TBD Game
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {}
  },
  methods: {
    scrollHandler(elm) {
      elm.scrollIntoView({ behavior: 'smooth', block: 'center' })
    },
    scrollToAbout() {
      const aboutView = document.getElementsByClassName('about')[0]
      this.scrollHandler(aboutView)
    },
    scrollToExperience() {
      const experienceView = document.getElementsByClassName('experience')[0]
      this.scrollHandler(experienceView)
    },
    scrollToProjects() {
      const projectsView = document.getElementsByClassName('projects')[0]
      this.scrollHandler(projectsView)
    },
    scrollToTBD() {
      const tbdView = document.getElementsByClassName('TBD')[0]
      this.scrollHandler(tbdView)
    },
  },
}
</script>

<style scoped>
.main-header-wrapper {
  display: flex;
  height: 5%;
  align-items: center;
  width: 100%;
  justify-content: space-between;
  /* background-color: black;
  opacity: 1; */
}
.nav-button-wrapper {
  color: white;
  text-shadow: -1px 0 black, 0 1px black, 1px 0 black, 0 -1px black;
  display: flex;
  justify-content: space-between;
  width: 30%;
  padding-right: 50px;
}
.header-icon {
  padding-left: 50px;
  height: 2em;
  color: white;
}
</style>
