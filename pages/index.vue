<template>
  <div class="container">
    <div class="wrapper">
      <div class="top-wrapper">
        <main class="main-wrapper">
          <div class="main-image">
            <Nav />
          </div>
          <div class="catch-copy">
            <div class="first">
              <h2>見える自然</h2>
            </div>
            <div class="second">
              <h2>見えない自然</h2>
            </div>
          </div>
        </main>
      </div>
      <div class="about-wrapper">
        <Title v-bind:titles="titles.about" />
        <div class="about-content-wrapper">
          <div class="about-main-image"></div>
          <div class="about-sub-content-wrapper">
            <div class="about-sub-image-wrapper">
              <div class="about-sub-image"></div>
            </div>
            <div class="about-sub-content">
              <div class="about-sub-content-text">
                <p>
                  現代美術を中心に、建築、写真、デザインなど、独自のコンセプトを打ち出している美術館。年に４回の企画展を開催している。併設のアートショップ「オンサンデーズ」には書籍から小物までスタイリッシュなアートグッズが豊富に揃う。
                </p>
                <p>
                  とくにポストカードの品揃えが充実。プレゼント探しにも利用できる。
                </p>
                <br />
                <p>個性的な企画展が魅力の現代美術館</p>
              </div>
              <div class="about-sub-content-link">
                <h2 class="about-link"><a href="#">アクセスはこちら</a></h2>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="exhibition-wrapper">
        <Title v-bind:titles="titles.exhibition" />
        <div class="exhibition-contents-wrapper">
          <div class="open-contents">
            <div class="open-title">開催中</div>
            <div class="open-wrapper">
              <div class="open-list-wrapper">
                <h3><a href="#">hoge</a></h3>
                <h3><a href="#">hoge</a></h3>
                <h3><a href="#">hoge</a></h3>
                <h3><a href="#">hoge</a></h3>
                <h3><a href="#">hoge</a></h3>
              </div>
              <div class="open-image"></div>
            </div>
          </div>
          <div class="close-contents">
            <div class="close-title">過去</div>
            <div class="close-wrapper">
              <div class="close-list-wrapper">
                <h3><a href="#">hoge</a></h3>
                <h3><a href="#">hoge</a></h3>
                <h3><a href="#">hoge</a></h3>
                <h3><a href="#">hoge</a></h3>
                <h3><a href="#">hoge</a></h3>
              </div>
              <div class="close-image"></div>
            </div>
          </div>
        </div>
      </div>
      <div class="lecture-wrapper">
        <Title v-bind:titles="titles.lecture" />
        <div class="lecture-contents-wrapper">
          <div class="open-contents">
            <div class="open-title">開催中</div>
            <div class="open-wrapper">
              <div class="open-list-wrapper">
                <h3><a href="#">hoge</a></h3>
                <h3><a href="#">hoge</a></h3>
                <h3><a href="#">hoge</a></h3>
                <h3><a href="#">hoge</a></h3>
                <h3><a href="#">hoge</a></h3>
              </div>
              <div class="open-image"></div>
            </div>
          </div>
          <div class="close-contents">
            <div class="close-title">過去</div>
            <div class="close-wrapper">
              <div class="close-list-wrapper">
                <h3><a href="#">hoge</a></h3>
                <h3><a href="#">hoge</a></h3>
                <h3><a href="#">hoge</a></h3>
                <h3><a href="#">hoge</a></h3>
                <h3><a href="#">hoge</a></h3>
              </div>
              <div class="close-image"></div>
            </div>
          </div>
        </div>
      </div>
      <div class="membership-wrapper">
        <Title v-bind:titles="titles.membership" />
        <div class="membership-contents-wrapper">
          <div class="membership-contents">
            <div class="image-wrapper">
              <div class="image-content-wrapper">
                <div class="membership-image"></div>
              </div>
            </div>
            <div class="membership-join-wrapper">
              <div class="membership-join-content">
                <h1><a href="#">申し込みはこちら</a></h1>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <a href="#" class="arrow"> </a>
  </div>
</template>

<script>
import Title from '../components/Title'
import Nav from '~/components/Nav.vue'
export default {
  components: {
    Nav,
    Title
  },
  data() {
    return {
      titles: {
        about: 'ワタリウム美術館について',
        exhibition: '展覧会一覧',
        lecture: 'レクチャー・ワークショップ一覧',
        membership: 'ワタリウムメンバーシップ'
      }
    }
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
    /*height: 500vh;*/

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
          background-image: url('~assets/images/saboten.jpg');
        }
        @media screen and (min-width: 376px) {
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
        @media screen and (max-width: 375px) {
          .main-image {
            width: 100vw;
          }
          .catch-copy {
            width: 38%;
            height: 10%;
            /*background-color: white;*/
            position: relative;
            top: -60%;
            right: -10%;

            .first {
              width: 100%;
              height: 50%;
              text-align: left;
              /*display: flex;*/
              /*align-items: center;*/
              /*background-color: lightgray;*/
              h2 {
                font-size: 18px;
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
                font-size: 18px;
              }
            }
          }
        }
      }
    }
    .about-wrapper {
      width: 100vw;
      height: 100vh;
      /*background-color: orange;*/
      .about-content-wrapper {
        height: 100%;
        width: 90%;
        margin: 0 auto;
        /*background-color: lightpink;*/
        display: flex;
        align-items: flex-start;
        /* mediaquery */
        /*flex-direction: column;*/
        .about-main-image {
          height: 80%;
          width: 45%;
          /*background-color: lightgoldenrodyellow;*/
          background-image: url('~assets/images/建物.png');
          background-size: 100%;
          background-repeat: no-repeat;
        }
        .about-sub-content-wrapper {
          height: 80%;
          width: 55%;
          /*background-color: lightskyblue;*/
          /*background-size: 100%;*/
          /*background-repeat: no-repeat;*/
          .about-sub-image-wrapper {
            height: 50%;
            width: 100%;
            @media screen and (max-width: 375px) {
              .about-sub-image-wrapper {
                /*height: 100%;*/
                /*width: 100%;*/
              }
            }
            /*background-color: lightcyan;*/
            .about-sub-image {
              height: 100%;
              width: 85%;
              /*background-color: lightcoral;*/
              margin: 0 auto;
              background-image: url('~assets/images/建物２.jpg');
              background-size: contain;
              background-repeat: no-repeat;
            }
          }
          .about-sub-content {
            height: 50%;
            width: 100%;
            /*background-color: lightseagreen;*/
            .about-sub-content-text {
              height: 75%;
              width: 85%;
              margin: 0 auto;
              /*background-color: lightpink;*/
              text-align: left;
              font-size: 20px;
            }
            @media screen and (max-width: 375px) {
              .about-sub-content-text {
                height: 75%;
                width: 95%;
                margin: 0 auto;
                /* background-color: lightpink; */
                text-align: left;
                font-size: 14px;
              }
              .about-sub-content-link {
                display: none;
              }
            }
            .about-sub-content-link {
              height: 25%;
              width: 85%;
              margin: 0 auto;
              /*background-color: lightgreen;*/
              text-align: left;
              position: relative;
              .about-link {
                position: absolute;
                bottom: 0;
                a {
                  text-decoration: none;
                  font-size: 35px;
                  margin-top: 10%;
                  color: #707070;
                  border-bottom: solid 2px #707070;
                }
              }
            }
          }
          @media screen and (max-width: 375px) {
            .about-sub-content {
              height: 50%;
              width: 197%;
              /* background-color: lightseagreen; */
              position: relative;
              right: 85%;
              top: 4%;
            }
          }
        }
      }
    }
    @media screen and (max-width: 375px) {
      .about-wrapper {
        height: 60vh;
      }
    }
    .exhibition-wrapper {
      width: 100vw;
      height: 100vh;
      /*background-color: orangered;*/

      .exhibition-contents-wrapper {
        width: 80%;
        height: 100%;
        /*background-color: lime;*/
        margin: 0 auto;

        .open-contents {
          width: 100%;
          height: 40%;
          /*background-color: orange;*/
          display: flex;
          flex-direction: column;
          .open-title {
            text-align: left;
            width: 100%;
            height: 10%;
            /*background-color: lightyellow;*/
            flex-direction: column;
          }
          .open-wrapper {
            width: 100%;
            height: 90%;
            /*background-color: lightseagreen;*/
            /*justify-content: flex-start;*/
            display: flex;
            justify-content: space-between;

            .open-list-wrapper {
              width: 45%;
              height: 100%;
              /*background-color: lightsalmon;*/
              text-align: left;
              h3 a {
                text-decoration: none;
                font-size: 47px;
                border-bottom: solid 2px #707070;
                color: #707070;
              }
            }

            .open-image {
              width: 55%;
              height: 100%;
              background-color: lightblue;
              background-image: url('~assets/images/exhibision_open.png');
              background-size: 105% 105%;
              background-repeat: no-repeat;
            }
            @media screen and (max-width: 375px) {
              .open-image {
                background-image: url('~assets/images/exhibision_open_sp.jpg');
              }
            }
          }
        }

        .close-contents {
          width: 100%;
          height: 40%;
          /*background-color: orange;*/
          display: flex;
          flex-direction: column;
          .close-title {
            width: 100%;
            height: 10%;
            /*background-color: lightyellow;*/
            flex-direction: column;
            text-align: left;
          }
          .close-wrapper {
            width: 100%;
            height: 90%;
            /*background-color: lightseagreen;*/
            /*justify-content: flex-start;*/
            display: flex;
            justify-content: space-between;

            .close-list-wrapper {
              text-align: left;
              width: 45%;
              height: 100%;
              /*background-color: lightsalmon;*/
              h3 a {
                text-decoration: none;
                font-size: 47px;
                border-bottom: solid 2px #707070;
                color: #707070;
              }
            }

            .close-image {
              width: 55%;
              height: 100%;
              background-color: lightblue;
              background-image: url('~assets/images/exhibision_close.png');
              background-size: 105% 105%;
              background-repeat: no-repeat;
            }
            @media screen and (max-width: 375px) {
              .close-image {
                background-image: url('~assets/images/exhibision_close_sp.jpg');
              }
            }
          }
        }
      }
    }

    .lecture-wrapper {
      width: 100vw;
      height: 100vh;
      /*background-color: yellowgreen;*/
      .lecture-contents-wrapper {
        width: 80%;
        height: 100%;
        /*background-color: lime;*/
        margin: 0 auto;

        .open-contents {
          width: 100%;
          height: 40%;
          /*background-color: orange;*/
          display: flex;
          flex-direction: column;
          .open-title {
            width: 100%;
            height: 10%;
            /*background-color: lightyellow;*/
            flex-direction: column;
            text-align: left;
          }
          .open-wrapper {
            width: 100%;
            height: 90%;
            /*background-color: lightseagreen;*/
            /*justify-content: flex-start;*/
            display: flex;
            justify-content: space-between;

            .open-list-wrapper {
              width: 45%;
              height: 100%;
              /*background-color: #e8f5fd;*/
              text-align: left;
              h3 a {
                text-decoration: none;
                font-size: 47px;
                border-bottom: solid 2px #707070;
                color: #707070;
              }
            }

            .open-image {
              width: 55%;
              height: 100%;
              background-image: url('~assets/images/lecture_open.png');
              background-size: 110% 110%;
              background-repeat: no-repeat;
              background-color: #e8f5fd;
            }
            @media screen and (max-width: 375px) {
              .open-image {
                background-image: url('~assets/images/lecture_open_sp.jpg');
                background-size: cover;
              }
            }
          }
        }

        .close-contents {
          width: 100%;
          height: 40%;
          /*background-color: orange;*/
          display: flex;
          flex-direction: column;
          .close-title {
            width: 100%;
            height: 10%;
            /*background-color: lightyellow;*/
            flex-direction: column;
            text-align: left;
          }
          .close-wrapper {
            width: 100%;
            height: 90%;
            /*background-color: #4eb2ae;*/
            /*justify-content: flex-start;*/
            display: flex;
            justify-content: space-between;

            .close-list-wrapper {
              width: 45%;
              height: 100%;
              /*background-color: lightsalmon;*/
              text-align: left;
              h3 a {
                text-decoration: none;
                font-size: 47px;
                border-bottom: solid 2px #707070;
                color: #707070;
              }
            }

            .close-image {
              width: 55%;
              height: 100%;
              background-image: url('~assets/images/osuman.png');
              background-size: 100% auto;
              background-repeat: no-repeat;
            }
            @media screen and (max-width: 375px) {
              .close-image {
                background-image: url('~assets/images/torajiro.jpg');
                background-size: cover;
              }
            }
          }
        }
      }
    }

    .membership-wrapper {
      width: 100vw;
      height: 100vh;
      /*background-color: lightskyblue;*/
      .membership-contents-wrapper {
        width: 100%;
        height: 80%;
        display: flex;
        /*background-color: lightpink;*/

        .membership-contents {
          width: 100%;
          height: 100%;
          /*background-color: orange;*/

          .image-wrapper {
            width: 100%;
            height: 80%;
            /*background-color: lightseagreen;*/

            .image-content-wrapper {
              height: 100%;
              width: 60%;
              /*background-color: lightyellow;*/
              margin: 0 auto;
              /*background-image: url('~assets/images/ワタリウムメンバーシップ.png');*/
              display: flex;
              align-items: center;
              .membership-image {
                height: 50%;
                width: 100%;
                background-image: url('~assets/images/ワタリウムメンバーシップ.png');
                /*background-color: black;*/
                background-size: contain;
                background-repeat: no-repeat;
              }
            }
          }
          .membership-join-wrapper {
            width: 100%;
            height: 20%;
            /*background-color: lightcyan;*/
            .membership-join-content {
              height: 100%;
              width: 60%;
              /*background-color: lightpink;*/
              margin: 0 auto;
              h1 {
                font-size: 50px;
                a {
                  text-decoration: none;
                  color: #707070;
                  border-bottom: solid #707070;
                }
              }
            }
            @media screen and (max-width: 375px) {
              .membership-join-content {
                h1 {
                  font-size: 28px;
                }
              }
            }
          }
          @media screen and (max-width: 375px) {
            .membership-join-wrapper {
              position: relative;
              top: -27%;
            }
          }
        }
      }
    }
    @media screen and (max-width: 375px) {
      .membership-wrapper {
        height: 45vh;
      }
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
