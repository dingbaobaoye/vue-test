<template>
  <header class="clearfix">
    <div class="logo fl">
      <img src="./assets/img/01-index-01.png" width="180">
    </div>
    <ul class="nav fr">
      <li>
        <router-link to="/">首页</router-link>
      </li>
      <li>
        <router-link to="/bracelet">北蓝手环</router-link>
      </li>
      <li>
        <router-link to="/service">服务支持</router-link>
        <div class="nav_hover nav_hover_bg fr hide">
          <div class="container_position">
            <ul class="nav_ul_1 fr">
              <li>
                <router-link to="/service/?type=1">产品购买</router-link>
              </li>
              <li>
                <router-link to="/service/?type=2">技术支持</router-link>
              </li>
              <li>
                <router-link to="/service/?type=3">维修服务</router-link>
              </li>
            </ul>
          </div>
        </div>
      </li>
      <li>
        <router-link to="/business">商务合作</router-link>
        <div class="nav_hover nav_hover_bg fr hide">
          <div class="container_position">
            <ul class="nav_ul_2 fr">
              <li>
                <router-link to="/business/">市场前景</router-link>
              </li>
              <li>
                <router-link to="/business/#about">联系我们</router-link>
              </li>
            </ul>
          </div>
        </div>
      </li>
      <li>
        <router-link to="/brand">智慧嘉孚</router-link>
      </li>
      <li>
        <router-link to="/app">APP下载</router-link>
      </li>
    </ul>
  </header>
</template>

<script>
  export default {
    name: 'head'
  }
</script>

<style scoped>
  header .nav>li a:hover{color:#0080db;}
  header .nav>li.active>a{color:#0080db;}
  header .nav_hover_bg {height: 50px;background: rgba(255,255,255,0.8);position: absolute;width: 100%;left: 0;z-index: 1;}
  header .container_position {position: relative;width: 1280px;margin: 0 auto;}
  header .nav_ul_1 {position: absolute;z-index: 99;top: 0;right: 335px;}
  header .nav_ul_2 {position: absolute;z-index: 99;top: 0;right: 245px;}
  header .nav_hover ul li {float: left;height: 50px;line-height: 50px;font-size: 15px;width: 85px;text-align: center;}
  header .nav_hover ul li a{font-size:13px;}
</style>
