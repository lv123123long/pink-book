<template>
  <div class="home-container">
    <swiper @swiper="onSwiper" @slideChange="onSlideChange" class="my-swiper">
    <swiper-slide>Slide 1</swiper-slide>
    <swiper-slide>Slide 2</swiper-slide>
    <swiper-slide>Slide 3</swiper-slide>
    ...
  </swiper>
  </div>
</template>

<script setup>
import { ref, reactive} from 'vue'
import {Swiper, SwiperSlide} from 'swiper/vue'
import 'swiper/css'

let mySwiper = null
const onSwiper = (swiper)=>{
  mySwiper = swiper
}
const onSlideChange = () =>{

}

</script>
<style scoped lang='scss'>
.home-container{
  .my-swiper{
    height: 100vh;
    background-color: rgb(249, 250, 249);
  }
}
</style>