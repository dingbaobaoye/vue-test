<template>
  <footer>
    <div class="container">
      <ul class="footer_nav clearfix">
        <li style="margin-left:0;padding-left:0;">
          <p>智慧嘉孚</p>
          <ul class="footer_text">
            <li><router-link to="/brand/#brand1">品牌介绍</router-link></li>
            <li><router-link to="/brand/#brand2">品牌理念</router-link></li>
            <li><router-link to="/brand/#brand3">品牌愿景</router-link></li>
          </ul>
        </li>
        <li class="border">
          <p>服务支持</p>
          <ul class="footer_text">
            <li><router-link to="/service/?type=1">产品购买</router-link></li>
            <li><router-link to="/service/?type=2">技术支持</router-link></li>
            <li><router-link to="/service/?type=3">维修服务</router-link></li>
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
              <img src="../assets/img/01-index-06.png" alt="">
              <div class="wx_two">
                <img src="../assets/img/01-index-09.png" alt="" height="130">
              </div>
            </div>
            <div class="wb fl">
              <img src="../assets/img/01-index-07.png" alt="">
              <div class="wb_two">
                <img src="../assets/img/01-index-10.png" alt="" height="130">
              </div>
            </div>
          </div>
        </li>
        <li style="padding-right:0;float:right;">
          <p>APP下载</p>
          <div class="app">
            <img src="../assets/img/01-index-08.png" alt="" width="52">
            <div class="app_two">

            </div>
          </div>
        </li>
      </ul>
    </div>
  </footer>
</template>

<script>

</script>

<style scoped>

  footer{min-width: 1280px;height:210px;background:#fff;border-top:1px solid #d4d4d4;box-shadow:0 -10px 20px #eee;}
  p{color:#26292d;line-height:50px;}
  .footer_nav{padding-top:25px;}
  .footer_nav>li{float:left;margin-left:35px;padding:0 30px;}
  .footer_nav>li.border{border-left:1px solid #d4d4d4;}
  .footer_nav>li:nth-child(5),footer .footer_nav>li:nth-child(6){margin-left:40px;}
  .footer_text li,footer .footer_text li a{color:#868686;font-size:14px;line-height:25px;}
  .wb{margin-left: 40px;}
  .wb,footer .wx,footer .app{position: relative;}
  .wx_two{position: absolute;top: -10px;left:-160px;display:none;z-index: 1}
  .wb_two{position: absolute;top:-10px;right:-160px;display:none;z-index: 1}
  .app_two{position: absolute;top: -10px;left:-160px;display:none;z-index: 1}
  .wb:hover .wb_two{display:block;}
  .wx:hover .wx_two{display:block;}
  .app:hover .app_two{display:block;}
</style>
