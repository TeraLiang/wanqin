<template>
  <div class="index">
    <!-- banner -->
    <img class="index__img" src="/image/banner.jpg" alt="">
    <!-- header -->
    <div class="index__header">
      <div class="index__header--title">晒作品</div>
      <div class="index__header--cont">专注与用心</div>
    </div>
    <!-- content -->
    <div class="index__content">

      <div class="index__content--body" @mouseover="showThis" @mouseleave="hideThis" @click="goDetails">
        <img class="content__body--img" src="/image/home.jpg" alt="">
        <!-- shade -->
        <div class="content__body--shade" v-show="show" >
          <div class="shade__title">向天歌训前纪律宣导</div>
          <div class="shade__cont">新的尝试</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name:'',
  data() {
    return{
      show : false
    }
  },
  methods:{
    showThis(){
      this.show = true
    },
    hideThis(){
      this.show = false
    },
    goDetails(){
      this.$router.push({path:'/details/one'})
    }
  }
}
</script>

<style scoped>
  .index__img{
    width: 100%;
  }
  .index__header{
    padding: 80px 0;
  }
  .index__header--title{
    color: #444;
    font-size: 26px;
    text-align: center;
  }
  .index__header--cont{
    color: #c1c1c1;
    font-size: 12px;
    text-align: center;
    line-height: 30px;
  }
  .index__content--body{
    width: 25%;
    cursor: pointer;
    position: relative;
  }
  .content__body--img{
    width: 100%;
  }
  .content__body--shade{
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.8);
    position: absolute;
    top: 0;
    left: 0;
    transition: all ease-out 0.3s;
  }
  .shade__title{
    position: relative;
    top: 50%;
    transform: translateY(-50%);
    color: #FFF;
    text-align: center;
    font-size: 14px;
  }
  .shade__cont{
    position: relative;
    top:50%;
    transform: translateY(-50%);
    color: #b7b7b7;
    text-align: center;
    font-size: 12px;
  }
</style>
