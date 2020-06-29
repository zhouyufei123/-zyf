<template>
  <div id="app">
    <section id="my-nr">
      <router-view></router-view>
    </section>
    <footer>
      <ul>
        <li><van-icon name="home-o" /><p><router-link to="/sy">首页</router-link></p></li>
        <li><van-icon name="home-o" /><p>分类</p></li>
        <li><van-icon name="home-o" /><p>购物车</p></li>
        <li><van-icon name="home-o" /><p>个人</p></li>
      </ul>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style lang="scss">
#app{
  font-size: .18rem;
  height: 100vh;
  width: 100vw;
  #my-nr{
    height: 90vh;
    overflow: auto;
  }
  footer{
    width: 100vw;
    height: 10vh;
    border-top: solid 1px gainsboro;
    box-sizing: border-box;
    ul{
      width: 100%;
      height: 100%;
      display: flex;
      align-items: center;
      li{
        width: 25%;
        text-align: center;
      }
    }
  }
}
</style>
