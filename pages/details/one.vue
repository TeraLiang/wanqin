<template>
  <div class="details">
    <div class="details__cont">

      <div class="details__cont--left">
        <img class="cont__left--img" src="/image/one/1.jpg" alt="">
        <img class="cont__left--img" src="/image/one/2.jpg" alt="">
        <img class="cont__left--img" src="/image/one/3.jpg" alt="">
      </div>

      <div class="details__cont--right">
        <div class="cont__right--title">向天歌训前纪律宣导</div>
        <div class="cont__right--cont">新的尝试</div>
        <div class="cont__right--hint"><span class="f-blue">用途：</span>MG动画宣传</div>
        <div class="cont__right--hint"><span class="f-blue">风格：</span>扁平化</div>
        <div>下载</div>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  name:'',
  data(){

  }
}
</script>

<style scoped>
  .f-blue{
    color: rgb(0 , 176, 240);
  }
  .details__cont{
    width: 1180px;
    margin: 0 auto;
    min-height: 600px;
  }
  .details__cont--left{
    float: left;
    width: 800px;
  }
  .cont__left--img{
    width: 100%;
    margin-bottom: 10px;
  }
  .details__cont--right{
    float: left;
    width: 340px;
    margin-left: 40px;
  }
  .cont__right--title{
    color: #444;
    font-size: 26px;
  }
  .cont__right--cont{
    color: #c1c1c1;
    font-size: 12px;
    line-height: 30px;
  }
  .cont__right--hint{
    
  }
</style>
