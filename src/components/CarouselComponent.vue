<template>
    <swiper
      :modules="modules"
      :slides-per-view="1"
      :space-between="50"
      navigation
      :pagination="{ clickable: true }"
      :scrollbar="{ draggable: true }"
      @swiper="onSwiper"
      @slideChange="onSlideChange"
    >
      <swiper-slide><img src="https://wallpapercave.com/wp/wp8788408.jpg" alt=""></swiper-slide>

      <swiper-slide><img src="https://wallpapercave.com/wp/wp2243047.jpg" alt=""></swiper-slide>

      <swiper-slide><img src="https://th.bing.com/th/id/R.e653e8d716df9c33b025ac5976d44555?rik=DK2pEnYR4B54bg&pid=ImgRaw&r=0" alt=""></swiper-slide>

      <swiper-slide><img src="https://wallpaper-house.com/data/out/12/wallpaper2you_578674.jpg" alt=""></swiper-slide>

      <swiper-slide><img src="https://images.designtrends.com/wp-content/uploads/2016/04/04071226/HD-Travel-Wallpaper.jpg" alt=""></swiper-slide>


      
      ...
    </swiper>
  </template>
  <script>
    // import Swiper core and required modules
    import { Navigation, Pagination, Scrollbar, A11y } from 'swiper';
  
    // Import Swiper Vue.js components
    import { Swiper, SwiperSlide } from 'swiper/vue';
  
    // Import Swiper styles
    import 'swiper/css';
    import 'swiper/css/navigation';
    import 'swiper/css/pagination';
    import 'swiper/css/scrollbar';
  
    // Import Swiper styles
    export default {
      components: {
        Swiper,
        SwiperSlide,
      },
      setup() {
        const onSwiper = (swiper) => {
          console.log(swiper);
        };
        const onSlideChange = () => {
          console.log('slide change');
        };
        return {
          onSwiper,
          onSlideChange,
          modules: [Navigation, Pagination, Scrollbar, A11y],
        };
      },
    };
  </script>

<style scooped>
    

</style>