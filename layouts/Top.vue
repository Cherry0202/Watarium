<template>
  <div class="top-wrapper">
    <main class="main-wrapper">
      main-wrapper
      <Nav />
    </main>
    top-wrapper
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
}
</style>
