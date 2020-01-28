<template>
  <div class="container">
    <div class="wrapper">
      <div class="top-wrapper">
        <main class="main-wrapper">
          <div class="main-image">
            <Nav />
          </div>
          <div class="catch-copy">
            <div class="first"><h2>見える自然</h2></div>
            <div class="second">
              <h2>見えない自然</h2>
            </div>
          </div>
        </main>
      </div>
      <div class="about-wrapper"></div>
      <div class="exhibition-wrapper"></div>
      <div class="lecture-wrapper"></div>
      <div class="membership-wrapper"></div>
    </div>
  </div>
</template>

<script>
import Nav from '~/components/Nav.vue'
export default {
  components: {
    Nav
  }
}
</script>

<style lang="scss">
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;

  .wrapper {
    /*background-color: antiquewhite;*/
    width: 100vw;
    height: 500vh;

    .top-wrapper {
      width: 100vw;
      height: 100vh;
      /*background-color: orange;*/

      .main-wrapper {
        width: 100vw;
        height: 95%;
        /*background-color: lightblue;*/

        .main-image {
          height: 100%;
          width: 90vw;
          background-size: cover;
        }

        .main-image {
        }

        .main-image {
          background-image: url('~assets/images/saboten.jpg');
        }

        .catch-copy {
          width: 40%;
          height: 35%;
          /*background-color: white;*/
          position: relative;
          top: -60%;
          right: -56%;
          .first {
            width: 100%;
            height: 50%;
            text-align: left;
            /*display: flex;*/
            /*align-items: center;*/
            /*background-color: lightgray;*/
            h2 {
              font-size: 83px;
            }
          }
          .second {
            width: 100%;
            height: 50%;
            /*top: 50%;*/
            text-align: right;
            /*vertical-align: middle;*/
            /*line-height: 50%;*/
            /*padding-top: 8%;*/
            /*background-color: lightyellow;*/
            h2 {
              font-size: 83px;
            }
          }
        }
      }
    }
    .about-wrapper {
      width: 100vw;
      height: 100vh;
      background-color: orange;
    }
    .exhibition-wrapper {
      width: 100vw;
      height: 100vh;
      background-color: orangered;
    }
    .lecture-wrapper {
      width: 100vw;
      height: 100vh;
      background-color: yellowgreen;
    }
    .membership-wrapper {
      width: 100vw;
      height: 100vh;
      background-color: lightskyblue;
    }
  }
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
