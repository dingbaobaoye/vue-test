<template>
  <section id="home">
    <div class="img_box t1">
      <router-link to="/bracelet/" style="display:block;height: 100%;"></router-link>
    </div>
    <div class="img_box t2"></div>
    <div class="img_box t3"></div>

    <div class="index_new">
      <div class="container">
        <div class="index_news_box">
          <p>行业资讯 <a href="/index/industry_list" class="fr more">更多&gt;&gt;</a></p>
          <ul class="clearfix">
            <li>
              <a href="/index/news_det?id=121">
                <span>2017-10-19</span>
                <div class="omit">高通正在开发下一代可穿戴芯片：努力降低智能手表的功耗</div>
              </a>
            </li>
            <li>
              <a href="/index/news_det?id=120">
                <span>2017-10-12</span>
                <div class="omit">实现穿戴设备真正价值 微软投身AI医疗项目</div>
              </a>
            </li>
            <li>
              <a href="/index/news_det?id=119">
                <span>2017-08-31</span>
                <div class="omit">三星发布两款可穿戴新品，主打游泳监测功能</div>
              </a>
            </li>
          </ul>
        </div>
        <div class="index_news_box" style="margin-top: 45px;border-top: 1px solid #f2f2f2;padding-top: 45px;">
          <p>嘉孚动态 <a href="/index/news_list" class="fr more">更多&gt;&gt;</a></p>
          <ul class="clearfix">

            <li>
              <a href="/index/news_det?id=116">
                <span>2017-07-25</span>
                <div class="omit">“自信 用心 创新” 相约金山城市沙滩</div>
              </a>
            </li>

            <li>
              <a href="/index/news_det?id=109">
                <span>2017-06-02</span>
                <div class="omit">嘉孚召开2017年第二季度职工动员会</div>
              </a>
            </li>

            <li>
              <a href="/index/news_det?id=104">
                <span>2017-04-25</span>
                <div class="omit">天气回暖 公司组织员工开展拓展训练活动</div>
              </a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>

</template>

<script>
export default {
  name: 'home',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .img_box{height:700px;background-size:1920px 700px;}
  .t1{background:url('../assets/img/01-index-03.jpg') no-repeat center;}
  .t2{background:url('../assets/img/01-index-04.jpg') no-repeat center;}
  .t3{background:url('../assets/img/01-index-05.jpg') no-repeat center;}
  .index_new{background:#fff;height:394px;}
  .index_new .container{padding:60px 0;}
  .index_new .index_news_box p{font-size:18px;color:#0080db;margin-bottom:30px;}
  .index_new .index_news_box li{float:left;padding:0 88px;width:397px;}
  .index_new .index_news_box li:first-child{padding-left:0;border:0;}
  .index_new .index_news_box li:nth-child(2){width:485px;}
  .index_new .index_news_box li:last-child{padding-right:0;}
  .index_new .index_news_box li a{color:#4c4c4c;}
  .index_new .more{color:#4c4c4c;font-size:14px;}
</style>
