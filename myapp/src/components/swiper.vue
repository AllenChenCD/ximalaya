<template>
 <div>
     <swiper :options="swiperOption" ref="mySwiper">
    <!-- slides -->
    <swiper-slide v-for="(item,index) in slide_img" :key="index">
      <img :src="item.imgurl" alt="">
    </swiper-slide>
    <!-- Optional controls -->
    <div class="swiper-pagination"  slot="pagination"></div>
    <!-- <div class="swiper-button-prev" slot="button-prev"></div>
    <div class="swiper-button-next" slot="button-next"></div> -->
    <!-- <div class="swiper-scrollbar"   slot="scrollbar"></div> -->
  </swiper>
 </div>
</template>

<script>
import "swiper/dist/css/swiper.css";
import { swiper, swiperSlide } from "vue-awesome-swiper";
import { sliders } from 'data/slidedata'



export default {
  name: "Swiper",
  data() {
    return {
      swiperOption: {
        notNextTick: true,
        loop: true,
        autoplay: {
          stopOnLastSlide: false
        },
        pagination: {
          el: ".swiper-pagination",
          clickable: true
        }
        
      },
      slide_img:[]
    };
  },
  computed: {},
  mounted() {
    this.slide_img = sliders
  },
  components: {
    swiper,
    swiperSlide
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
