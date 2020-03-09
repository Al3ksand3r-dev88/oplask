<template>
  <div>
    <Search @get-images="getImages" />
    <Lightbox :imageArray="imageArray" />
    <Gallery @open-modal="openModal" :imageArray="imageArray" />
  </div>
</template>

<script>
import Lightbox from "@/components/Lightbox.vue";
import Gallery from "@/components/Gallery.vue";
import Search from "@/components/Search.vue";
export default {
  name: "App",
  components: {
    Lightbox,
    Gallery,
    Search
  },
  data() {
    return {
      imageArray: []
    };
  },
  methods: {
    getImages(getImages) {
      this.imageArray = getImages;
    },
    openModal() {}
  }
};
</script>
<style lang="scss" scoped>
@import url("https://fonts.googleapis.com/css?family=Poppins&display=swap");

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;

  font-family: "Poppins", sans-serif;
  .wrapper {
    display: flex;
    width: 100%;
    height: 100vh;
  }
}
</style>
