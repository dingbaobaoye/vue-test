<template>
  <header>
    <div class="container clearfix">
      <div class="fl logo">
        <img src="../assets/img/01-index-01.png" alt="" width="180">
      </div>
      <ul class="nav clearfix fr">
        <li class="active">
          <router-link to="index">首页</router-link>
        </li>
        <li>
          <router-link to="bracelet">北蓝手环</router-link>
        </li>
        <li>
          <router-link to="service">服务支持</router-link>
          <head-nav></head-nav>
        </li>
        <li>
          <router-link to="scenarios">商务合作</router-link>
          <head-nav></head-nav>
        </li>
        <li>
          <router-link to="brand">智慧嘉孚</router-link>
        </li>
        <li>
          <router-link to="app">APP下载</router-link>
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
  import Vue from 'vue';
  import headNav from '../components/head_nav';
  export default {
    name: 'head',
    components: {
      headNav
    }
  }

</script>

<style scoped>
  header{min-width: 1280px;height:80px;text-align: center;position:fixed;top:0;left:0;width:100%;z-index:999;background: #fff;}
  .logo{height:80px;margin:15px 0;}
  .nav{margin:0 auto;}
  .nav>li{float:left;line-height:80px;}
  .nav>li:nth-child(2n+1){width:140px;}
  .nav>li>a{display:block;height:100%;padding:0 32px;}
  .nav>li a:hover{color:#0080db;}
  .nav>li.active>a{color:#0080db;}

</style>
