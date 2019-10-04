<template>
  <div class="main-header-wrapper">
    <img
      class="header-icon"
      src="../../public/images/FunPlus_Phoenix_logo.png"
    >
    <div class="nav-button-wrapper">
      <div>/- ONE - /</div>
      <div>/- TWO - /</div>
      <div>/- THREE - /</div>
      <div>/- FOUR - /</div>
      <div>/- FIVE - /</div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.main-header-wrapper {
  display: flex;
  height: 5%;
  align-items: center;
  width: 100%;
  justify-content: space-between;
}
.nav-button-wrapper {
  color: white;
  text-shadow: -1px 0 black, 0 1px black, 1px 0 black, 0 -1px black;
  display: flex;
  padding-right: 50px;
}
.header-icon {
  padding-left: 50px;
  height: 2em;
}
</style>
