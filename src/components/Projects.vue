<template>
  <Carousel
    class="w-11/12 mx-auto"
    :autoplay="2000"
    :itemsToShow="3.95"
    :wrapAround="true"
    :transition="500"
  >
    <Slide class="bg-blue-500" v-for="slide in 4" :key="slide">
      <div class="carousel__item">{{ slide }}</div>
    </Slide>
    <template #addons>
      <navigation />
      <pagination />
    </template>
  </Carousel>
</template>

<script>
import "vue3-carousel/dist/carousel.css";
import { Carousel, Pagination, Slide, Navigation } from "vue3-carousel";
export default {
  components: { Carousel, Slide, Pagination, Navigation },
};
</script>
<style scoped>
.carousel__slide {
  padding: 5px;
  height: 20rem;
}

.carousel__viewport {
  perspective: 2000px;
}

.carousel__track {
  transform-style: preserve-3d;
}

.carousel__slide--sliding {
  transition: 0.5s;
}

.carousel__slide {
  opacity: 0.9;
  transform: rotateY(-20deg) scale(0.9);
}

.carousel__slide--active ~ .carousel__slide {
  transform: rotateY(20deg) scale(0.9);
}

.carousel__slide--prev {
  opacity: 1;
  transform: rotateY(-10deg) scale(0.95);
}

.carousel__slide--next {
  opacity: 1;
  transform: rotateY(10deg) scale(0.95);
}

.carousel__slide--active {
  opacity: 1;
  transform: rotateY(0) scale(1.1);
}
</style>
