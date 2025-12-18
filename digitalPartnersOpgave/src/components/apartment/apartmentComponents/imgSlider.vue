<script setup>
import { boliger } from "../../../data/data";
import { onMounted } from 'vue';
onMounted(() => {
  const swiper = new Swiper('.swiper', {

    // Hvis flere slides skal vises ad gangen
    slidesPerView: 3,
    spaceBetween: 116,

    // Optional parameters
    direction: 'horizontal',
    loop: true,

    // If we need pagination
    pagination: {
      el: '.swiper-pagination',
    },

    // Navigation arrows
    navigation: {
      nextEl: '.swiper-button-next',
      prevEl: '.swiper-button-prev',
    }
  });
});
</script>

<template>
  <!-- Slider main container -->
  <div class="swiper">
    <!-- Additional required wrapper -->
    <div class="swiper-wrapper">
      <!-- Slides -->
      <div class="swiper-slide" v-for="(image, index) in boliger[0].images" :key="index">
        <img :src="image" alt="">
      </div>
    </div>
    <!-- If we need pagination -->
    <div class="swiper-pagination"></div>

    <!-- If we need navigation buttons -->
    <div class="swiper-button-prev"></div>
    <div class="swiper-button-next"></div>
  </div>
</template>

<style scoped>
img {
  width: clamp(400px, 33vw, 800px);
  height: 500px;
  object-fit: cover;
  border-radius: 10px;
}

.swiper {
  width: 100%;
  margin-top: 16px;
}

.swiper-slide {
  display: flex;
  justify-content: center;
}
</style>