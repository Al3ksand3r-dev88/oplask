<template>
  <div>
    <carousel class="carousel-slider">
      <slide>Slide 1 Content</slide>
      <slide>Slide 2 Content</slide>
    </carousel>
  </div>
</template>

<script>
import { Carousel, Slide } from "vue-carousel";


export default {
  name: "Lightbox",
  components: {
    Carousel,
    Slide,
   
  }
};
</script>

<style lang="scss" scoped>
.VueCarousel-slide {
  color: red;
}

.VueCarousel-dot-container {
  color: blue;
}
</style>