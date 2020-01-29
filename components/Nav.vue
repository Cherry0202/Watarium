<template>
  <nav class="nav">
    <ul>
      <li class="logo"></li>
      <li class="menu"><a href="#">ワタリウム美術館について</a></li>
      <li class="menu"><a href="#">展覧会一覧</a></li>
      <li class="menu"><a href="#">レクチャー・ワークショップ一覧</a></li>
      <li class="menu"><a href="#">ワタリウムメンバーシップ</a></li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'Nav'
}
</script>

<style scoped lang="scss">
/**list-styleを指定する**/
* {
  margin: 0;
  padding: 0;
}

nav {
  width: 100vw;
  margin: auto;
  padding: 0;
  /*background-color: lightskyblue;*/

  ul {
    margin: 0;
    padding: 0;
    display: -webkit-flex;
    display: flex;
    list-style: none;

    li.logo {
      width: 300px;
      margin: 0;
      padding: 0;
      border-radius: 5px;
      line-height: 1;
      color: #000;
      font-size: 20px;
      /*background: #007bbb;*/
      /*background-image: url('~assets/images/watarium_logo.png');*/
      /*background-size: cover;*/
      height: 110px;
      /*width: 417px;*/
    }

    @media screen and (min-width: 376px) {
      li.menu {
        width: 239px;
        margin: 0;
        padding: 0;
        border-radius: 5px;
        line-height: 1;
        color: #000;
        font-size: 15px;
        /*background: #007bbb;*/
        height: 110px;
        display: flex;
        justify-content: center;
        align-items: center;
        /*width: 417px;*/
      }
    }

    @media screen and (max-width: 375px) {
      li.menu {
        display: none;
      }
    }

    li:first-child {
      margin-right: auto;
      background-image: url('~assets/images/watariumu_logo_new.png');
      background-size: contain;
      background-repeat: no-repeat;
      width: 417px;
    }

    li a {
      display: block;
      margin: 0;
      padding: 0;
      color: #000;
      text-decoration: none;
      font-weight: 400;
    }
  }
}
</style>
