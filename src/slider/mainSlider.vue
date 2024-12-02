<template>
  <swiper :spaceBetween="30" :centeredSlides="true" :autoplay="{
    delay: 8000,
    disableOnInteraction: false,
  }" :pagination="{
        clickable: true,
      }" :navigation="true" :modules="modules" class="mySwiper">
    <swiper-slide>
      <SliderItemOne/>
    </swiper-slide>
    <swiper-slide>
    <SliderItemTwo/>
    </swiper-slide>
    <swiper-slide>
      <iframe width="100%" height="500" src="https://www.youtube.com/embed/VJI1bcoilT4?si=AWk1gSrXmS2Uqw55" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </swiper-slide>
    <swiper-slide>
      <img src="./img/image 6.png" alt="">
    </swiper-slide>
  </swiper>
</template>
<script>
// Import Swiper Vue.js components
import SliderItemOne from './SliderItemOne.vue';
import SliderItemTwo from './SliderItemTwo.vue';
import { Swiper, SwiperSlide } from 'swiper/vue';
// Import Swiper styles
import 'swiper/css';

import 'swiper/css/pagination';
import 'swiper/css/navigation';

import './style.css';

// import required modules
import { Autoplay, Pagination, Navigation } from 'swiper/modules';

export default {
  components: {
    Swiper,
    SwiperSlide,
    SliderItemOne,
    SliderItemTwo,
  },
  setup() {
    return {
      modules: [Autoplay, Pagination, Navigation],
    };
  },
};
</script>