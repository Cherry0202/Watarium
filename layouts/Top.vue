<template>
  <div class="top-wrapper">
    <main class="main-wrapper">
      <div class="main-image">
        <Nav />
      </div>
    </main>
  </div>
</template>

<script>
import Nav from '../components/Nav'
export default {
  components: { Nav }
}
</script>

<style scoped lang="scss">
.top-wrapper {
  width: 100vw;
  height: 1080px;
  background-color: orange;
  .main-wrapper {
    width: 100vw;
    height: 1030px;
    background-color: lightblue;
  }
  .main-image {
    height: 1030vh;
    width: 75vw;
    background-color: lightpink;
  }
}
</style>
