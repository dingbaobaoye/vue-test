<template>
  <div id="app">
    <header class="clearfix">

    </header>
    <img src="./assets/img/01-index-01.png" width="180">
    <ul>
      <li>首页</li>
      <li>北蓝手环</li>
      <li>服务支持</li>
      <li>商务合作</li>
      <li>智慧嘉孚</li>
      <li>APP下载</li>
    </ul>
    <router-view></router-view>
  </div>
</template>

<script>
  export default {
    name: 'app'
  }
</script>

<style src="./src/assets/css/base.css"></style>
<style>
#app {
  font-family: '微软雅黑', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width:1200px;
  margin:auto;
}
.clearfix{

}
img{float:left;}
ul{float:left;}
ul li{float:left;}
</style>
