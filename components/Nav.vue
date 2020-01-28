<template>
  <nav class="nav">
    nav
    <ul>
      <li><a href="#">LOGO</a></li>
      <li><a href="#">List1</a></li>
      <li><a href="#">List2</a></li>
      <li><a href="#">List3</a></li>
      <li><a href="#">List4</a></li>
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
  max-width: 85vw;
  margin: auto;
  padding: 0;

  ul {
    margin: 0;
    padding: 0;
    display: -webkit-flex;
    display: flex;
    list-style: none;

    li {
      margin: 15px;
      padding: 0;
      border-radius: 5px;
      line-height: 1;
      color: #fff;
      background: #007bbb;
      height: 110px;
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
      padding: 20px;
      color: #fff;
      text-decoration: none;
    }
  }
}
</style>
