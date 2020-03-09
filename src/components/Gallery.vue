<template>
  <div>
    <div class="gallery-container">
      <ul>
        <li v-for="image in imageArray.results" :key="image.id">
          <div
            class="image-box"
            :style="{ backgroundImage: `url(${image.urls.small})` }"
          />
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "Gallery",
  props: ["imageArray"]
};
</script>

<style lang="scss" scoped>
.gallery-container {
  width: 960px;
  margin: auto;
  ul {
    gap: 2rem;
    margin: 4rem 0;
    display: grid;
    list-style: none;
    grid-template-columns: repeat(3, 1fr);
    li {
      cursor: pointer;
      .image-box {
        width: 300px;
        height: 300px;
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
      }
    }
  }
}
</style>
