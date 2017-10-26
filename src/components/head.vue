<template>
  <header>
    <div class="container clearfix">
      <div class="fl logo">
        <img src="../assets/img/01-index-01.png" alt="" width="180">
      </div>
      <ul class="nav clearfix fr">
        <li v-for="item in items" v-bind:class="{ active : item.active }" @click="click(item)" @mouseenter="show(item)" @mouseleave="hidden(item)">
          <router-link v-bind:to="item.url">{{item.text}}</router-link>
          <div class="nav_hover nav_hover_bg fr" v-if="item.select" v-show="item.isHover">
            <div class="container_position">
              <ul v-show="item.isFirst" class="nav_ul_1 fr">
                <li><router-link to="service">产品购买</router-link></li>
                <li><router-link to="service">技术支持</router-link></li>
                <li><router-link to="service">维修服务</router-link></li>
              </ul>
              <ul v-show="!item.isFirst" class="nav_ul_2 fr">
                <li><router-link to="scenarios">市场前景</router-link></li>
                <li><router-link to="scenarios">联系我们</router-link></li>
              </ul>
            </div>
          </div>
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
  import Vue from 'vue';
  export default {
    name: 'head',
    data () {
      return {
        items: [
          {
            text: '首页',
            url: '/',
            select: false,
            active: true
          },{
            text: '北蓝手环',
            url: '/bracelet',
            select: false,
            active: false
          },{
            text: '服务支持',
            url: '/service',
            select: true,
            active: false,
            isFirst: true,
            isHover: false
          },{
            text: '商务合作',
            url: '/scenarios',
            select: true,
            active: false,
            isFirst: false,
            isHover: false
          },{
            text: '智慧嘉孚',
            url: '/brand',
            select: false,
            active: false
          },{
            text: 'APP下载',
            url: '/app',
            select: false,
            active: false
          }
        ]
      }
    },
    methods: {
      show (item) {
        this.items.forEach(function(li){
          li.isHover = false;
        })
        item.isHover = true;
      },
      hidden (item) {
        this.items.forEach(function(li){
          li.isHover = false;
        })
      },
      click (item) {
        this.items.forEach(function(item){
          item.active = false;
        })
        item.active = true;
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
  .nav>li a:hover{color:#0080db;}
  .nav>li.active>a{color:#0080db;}
</style>
