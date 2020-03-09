<template>

  <div>
      <Search />
    <Lightbox />
    <Gallery />
    <Pager />

  </div>
</template>

<script>
import Lightbox from "@/components/Lightbox.vue";
import Gallery from "@/components/Gallery.vue";
import Search from '@/components/Search.vue'; 
import Pager from '@/components/Pager.vue'; 

export default {
  name: "App",
  components: {
    Lightbox,
    Gallery,
    Search,
    Pager
  }
}  
</script>
<style lang="scss" scoped>
@import url("https://fonts.googleapis.com/css?family=Poppins&display=swap");

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;

  font-family: "Poppins", sans-serif;
  .wrapper{
  display: flex;
  width: 100%;
  height: 100vh;
  }
}

</style>
