<template>
  <div id="app">
    <!--<my-head></my-head>-->

    <router-view></router-view>

    <footer>
      <ul class="footer_nav clearfix">
        <li style="margin-left:0;padding-left:0;">
          <p>智慧嘉孚</p>
          <ul class="footer_text">
            <li><a href="/brand/#brand1">品牌介绍</a></li>
            <li><a href="/brand/#brand2">品牌理念</a></li>
            <li><a href="/brand/#brand3">品牌愿景</a></li>
          </ul>
        </li>
        <li class="border">
          <p>服务支持</p>
          <ul class="footer_text">
            <li><a href="/service/?type=1">产品购买</a></li>
            <li><a href="/service/?type=2">技术支持</a></li>
            <li><a href="/service/?type=3">维修服务</a></li>
          </ul>
        </li>
        <li class="border">
          <p>战略伙伴</p>
          <ul class="footer_text">
            <li><a href="http://www.shfzwkeji.com" target="_blank">上海方芝维信息科技有限公司</a></li>
            <li><a href="http://www.yuanjindianzi.com" target="_blank">上海圆津电子科技有限公司</a></li>
            <li><a href="http://www.shanghaijuean.com" target="_blank">上海爵安股权投资基金有限公司</a></li>
          </ul>
        </li>
        <li class="border">
          <p>联系我们</p>
          <ul class="footer_text">
            <li class="addr">地址：上海市联航路1688弄17号楼C座</li>
            <li class="tel">电话：021-31605147</li>
            <li class="mail">邮箱：<a href="mailto:jiafukejixinxi@163.com">jiafukejixinxi@163.com</a></li>
          </ul>
        </li>
        <li>
          <p>关注我们</p>
          <div>
            <div class="wx fl">
              <img src="./assets/img/01-index-06.png" alt="">
              <div class="wx_two">
                <img src="./assets/img/01-index-09.png" alt="" height="130">
              </div>
            </div>
            <div class="wb fl">
              <img src="./assets/img/01-index-07.png" alt="">
              <div class="wb_two">
                <img src="./assets/img/01-index-10.png" alt="" height="130">
              </div>
            </div>
          </div>
        </li>
        <li style="padding-right:0;float:right;">
          <p>APP下载</p>
          <div class="app">
            <img src="./assets/img/01-index-08.png" alt="" width="52">
            <div class="app_two">

            </div>
          </div>
        </li>
      </ul>
    </footer>
  </div>
</template>

<script>
//  import myHead from './components/head.vue'
  export default {
    name: 'app',
//    components: {'my-head': myHead}
  }
</script>

<style src="./assets/css/base.css"></style>
<style>
  #app {
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
  }
  a{color: #26292d;}
  header{
    margin: auto;
    width:1280px;
  }
  .logo{
    padding:15px 0;
  }
  .nav>li{
    float:left;
    line-height: 80px;
  }
  .nav>li>a{
    display: block;
    height: 100%;
    padding: 0 32px;
  }

  header .nav>li a:hover{color:#0080db;}
  header .nav>li.active>a{color:#0080db;}
  header .nav_hover_bg {height: 50px;background: rgba(255,255,255,0.8);position: absolute;width: 100%;left: 0;z-index: 1;}
  header .container_position {position: relative;width: 1280px;margin: 0 auto;}
  header .nav_ul_1 {position: absolute;z-index: 99;top: 0;right: 335px;}
  header .nav_ul_2 {position: absolute;z-index: 99;top: 0;right: 245px;}
  header .nav_hover ul li {float: left;height: 50px;line-height: 50px;font-size: 15px;width: 85px;text-align: center;}
  header .nav_hover ul li a{font-size:13px;}

  footer{height:210px;background:#fff;border-top:1px solid #d4d4d4;box-shadow:0 -10px 20px #eee;}
  footer p{color:#26292d;line-height:50px;}
  footer .footer_nav{padding-top:25px;width: 1280px;margin:auto;}
  footer .footer_nav>li{float:left;margin-left:35px;padding:0 30px;}
  footer .footer_nav>li.border{border-left:1px solid #d4d4d4;}
  footer .footer_nav>li:nth-child(5),footer .footer_nav>li:nth-child(6){margin-left:40px;}
  footer .footer_text li,footer .footer_text li a{color:#868686;font-size:14px;line-height:25px;}
  footer .wb{margin-left: 40px;}
  footer .wb,footer .wx,footer .app{position: relative;}
  footer .wx_two{position: absolute;top: -10px;left:-160px;display:none;z-index: 1}
  footer .wb_two{position: absolute;top:-10px;right:-160px;display:none;z-index: 1}
  footer .app_two{position: absolute;top: -10px;left:-160px;display:none;z-index: 1}
  footer .wb:hover .wb_two{display:block;}
  footer .wx:hover .wx_two{display:block;}
  footer .app:hover .app_two{display:block;}
</style>
