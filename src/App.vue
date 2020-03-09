<template>
  <div>
    <Lightbox />
    <Gallery />
  </div>
</template>

<script>
import Lightbox from "@/components/Lightbox.vue";
import Gallery from "@/components/Gallery.vue";

export default {
  name: "App",
  components: {
    Lightbox,
    Gallery
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
}
</style>
