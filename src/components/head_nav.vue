<template>
    <div class="nav_hover nav_hover_bg fr" v-show="isActive">
      <div class="container_position">
        <ul v-bind:class="[isFirst ? 'nav_ul_1' : 'nav_ul_2' , 'fr'] ">
          <li><router-link to="scenarios">市场前景</router-link></li>
          <li><router-link to="scenarios">联系我们</router-link></li>
        </ul>
      </div>
    </div>
</template>

<script>
  export default {
    data() {
      return {
        isActive : true,
        isFirst : false
      }
    }
  }
</script>

<style scoped>
  .nav_hover_bg {height: 50px;background: rgba(255,255,255,0.8);position: absolute;width: 100%;left: 0;z-index: 1;}
  .container_position {position: relative;width: 1280px;margin: 0 auto;}
  .nav_ul_1 {position: absolute;z-index: 99;top: 0;right: 335px;}
  .nav_ul_2 {position: absolute;z-index: 99;top: 0;right: 245px;}
  .nav_hover ul li {float: left;height: 50px;line-height: 50px;font-size: 15px;width: 85px;text-align: center;}
  .nav_hover ul li a{font-size:13px;}
  .nav>li a:hover{color:#0080db;}
  .nav>li.active>a{color:#0080db;}
</style>
