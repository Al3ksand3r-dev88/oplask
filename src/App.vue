<template>
<div class="wrapper">
  <Search />
</div>
</template>

<script>
import Search from './components/Search.vue' 
export default {
  name: "App",
  components:{
    Search,
  }
};
</script>

<style lang="scss" >
.wrapper{
  display: flex;
  width: 100%;
  height: 100vh;
}
</style>
