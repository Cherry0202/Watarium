<template>
  <div class="head-wrapper">
    <div class="title-wrapper">
      <h1>{{ titles }}</h1>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Title',
  props: {
    titles: {
      type: Object
    }
  }
}
</script>

<style scoped lang="scss">
.head-wrapper {
  width: 100vw;
  height: 20vh;
  background-color: whitesmoke;
  display: flex;
  align-items: center;
  .title-wrapper {
    height: 45%;
    width: 45%;
    h1 {
      font-size: 40px;
      font-weight: 400;
      border-top: solid 2px #000000;
      border-bottom: solid 2px #000000;
    }
  }
  @media screen and (max-width: 375px) {
    height: 10vh;
    .title-wrapper {
      h1 {
        font-size: 14px;
        font-weight: 200;
        border-top: solid 1px #000000;
        border-bottom: solid 1px #000000;
      }
    }
  }
}
</style>
