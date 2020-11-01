<template>
  <div class="construction-container">
    <div class="construction-text">
      <div>CURRENTLY UNDER CONSTRUCTION!</div>
      <div>SORRY FOR THE INCONVENIENCE!</div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.construction-container {
  display: flex;
  justify-content: center;
  align-items: center;
}
.construction-text {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100%;
  width: 60%;
  font-size: 1.5em;
  text-shadow: -2px 0 black, 0 2px black, 2px 0 black, 0 -2px black;
}
</style>
