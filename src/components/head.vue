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
          <div class="nav_hover nav_hover_bg fr" v-show="isActive">
            <div class="container_position">
              <ul class="nav_ul_1 fr">
                <li><router-link to="service">产品购买</router-link></li>
                <li><router-link to="service">技术支持</router-link></li>
                <li><router-link to="service">维修服务</router-link></li>
              </ul>
            </div>
          </div>
        </li>
        <li>
          <router-link to="scenarios">商务合作</router-link>
          <div class="nav_hover nav_hover_bg fr" v-show="isActive">
            <div class="container_position">
              <ul class="nav_ul_2 fr">
                <li><router-link to="scenarios">市场前景</router-link></li>
                <li><router-link to="scenarios">联系我们</router-link></li>
              </ul>
            </div>
          </div>
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
    export default {
        data() {
          return {
            isActive : true
          }
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
  .nav_hover_bg {height: 50px;background: rgba(255,255,255,0.8);position: absolute;width: 100%;left: 0;z-index: 1;}
  .container_position {position: relative;width: 1280px;margin: 0 auto;}
  .nav_ul_1 {position: absolute;z-index: 99;top: 0;right: 335px;}
  .nav_ul_2 {position: absolute;z-index: 99;top: 0;right: 245px;}
  .nav_hover ul li {float: left;height: 50px;line-height: 50px;font-size: 15px;width: 85px;text-align: center;}
  .nav_hover ul li a{font-size:13px;}
</style>
