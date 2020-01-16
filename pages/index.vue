<template>
  <div class="container">
    <div class="wrapper">
      <!--      <Nav />-->
      <Top />
    </div>
  </div>
</template>

<script>
import Top from '~/components/Top.vue'
// import Nav from '~/components/Nav.vue'
export default {
  components: {
    Top
    // Nav
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.wrapper {
  background-color: antiquewhite;
  width: 1920px;
  height: 6054px;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
