<template>
  <div class="home">
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <h4>多加网</h4>
    <p><input type="text" placeholder="热门搜索"/></p>
    <div class="lbt">
       <swiper :options="swiperOption">
         <swiper-slide>
           111
         </swiper-slide>
          <swiper-slide>
          222
         </swiper-slide>
          <swiper-slide>
           333
         </swiper-slide>
       </swiper>
    </div>
    <div class="main"></div>
    <div class="count"></div>
  </div>
</template>

<script>
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  components: {
    HelloWorld
  },
  data(){
    return {
      swiperOption: {
        autoplay: true
      }
    }
  }
}
</script>
<style lang="scss" scoped>
  .home{
    flex: l;
    height: 100%;
    width: 100%;
    h4{
      width: 100%;
      line-height: 40px;
      text-align: center;
      background: rgba($color: #000000, $alpha: 0.9);
      color: #fff;
    }
    p{
       width: 100%;
       height: 40px;
      background: seagreen;
      padding: 5px;
      input{
        width: 100%;
        height: 100%;
        outline: none;
        border: none;
        border-radius: 20px;
      }
    }
    .lbt{
      width: 100%;
      height: 150px;
    }
    .main{
      width: 100%;
      height: 150px;
      background: skyblue;
    }
    .count{
      width: 100%;
      height: 225px;
      background: darkolivegreen;
    }
  }
</style>
