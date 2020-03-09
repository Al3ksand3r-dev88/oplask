<template>
  <div>
    <carousel :class="{open: isClicked}" class="carousel-slider" perPage="1">
      <slide v-for="image in imageArray.results" :key="image.id">
        <img :src="image.urls.small" />
      </slide>
    </carousel>
  </div>
</template>

<script>
import { Carousel, Slide } from "vue-carousel";

export default {
  name: "Lightbox",
  props: ["imageArray"],
  components: {
    Carousel,
    Slide
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