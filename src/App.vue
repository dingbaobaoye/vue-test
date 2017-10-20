<template>
  <div id="app">
    <my-head></my-head>
    <router-view></router-view>
    <my-foot></my-foot>
  </div>
</template>

<script>
  import Vue from 'vue';
  import myHead from './components/head';
  import myFoot from './components/foot';

//  new Vue({
//    el: '#app'
//  });
  export default {
    name: 'app',
    components: {
      myHead, myFoot
    }
  }
</script>

<style src="./assets/css/base.css"></style>
<style>
  body{min-width:1280px;padding-top:80px;}
  .container{width:1280px;margin:0 auto;}
  a{color:#26292d;}
  .hide{display:none;}
  .omit{overflow: hidden;text-overflow:ellipsis;white-space: nowrap;}
</style>
