<template>
  <div class="home">
    <div class="img_box bg1">
      <router-link to="/bracelet">北蓝手环</router-link>
    </div>
    <div class="img_box bg2"></div>
    <div class="img_box bg3"></div>
  </div>
</template>

<script>
export default {
  name: 'home',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .img_box {
    height: 700px;
  }
  .bg1 {
    background:url('../assets/img/01-index-03.jpg') no-repeat center;background-size:1920px 700px;
  }
  .bg2 {
    background:url('../assets/img/01-index-04.jpg') no-repeat center;background-size:1920px 700px;
  }
  .bg3 {
    background:url('../assets/img/01-index-05.jpg') no-repeat center;background-size:1920px 700px;
  }
  a {display:block;height: 100%;}
</style>
