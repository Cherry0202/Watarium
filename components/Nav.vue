<template>
  <nav class="nav">
    <ul>
      <li class="logo"><a href="#">LOGO</a></li>
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
  background-color: lightskyblue;

  ul {
    margin: 0;
    padding: 0;
    display: -webkit-flex;
    display: flex;
    list-style: none;

    li.logo {
      width: 300px;
      margin: 0px;
      padding: 0;
      border-radius: 5px;
      line-height: 1;
      color: #fff;
      font-size: 20px;
      background: #007bbb;
      height: 110px;
      /*width: 417px;*/
    }

    li.menu {
      width: 239px;
      margin: 0px;
      padding: 0;
      border-radius: 5px;
      line-height: 1;
      color: #fff;
      font-size: 15px;
      background: #007bbb;
      height: 110px;
      display: flex;
      justify-content: center;
      align-items: center;
      /*width: 417px;*/
    }

    li:first-child {
      margin-right: auto;
      background: #f8b500;
      width: 417px;
    }

    li a {
      display: block;
      margin: 0;
      padding: 0;
      color: #fff;
      text-decoration: none;
    }
  }
}
</style>
