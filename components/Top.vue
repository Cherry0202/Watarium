<template>
  <div class="top-wrapper">
    <Nav />
  </div>
</template>

<script>
import Nav from './Nav'
export default {
  components: { Nav }
}
</script>

<style scoped lang="scss">
.top-wrapper {
  width: 100vw;
  height: 1080px;
  background-color: orange;
}
</style>
