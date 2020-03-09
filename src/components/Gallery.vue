<template>
  <div>
<div class="gallery-container">
<ul>
  <li>1</li>
  <li>2</li>
  <li>3</li>
  <li>4</li>
  <li>5</li>
  <li>6</li>
  <li>7</li>
  <li>8</li>
  <li>9</li>
</ul>
</div>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  name: "Gallery"
};
</script>

<style lang="scss" scoped>
.gallery-container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: repeat(3, 1fr);

  height: 100vh;
  width: 80%;
  margin: auto;
  z-index: 100;
  position: absolute;
  margin-top: 45rem;
  margin-left: 8.5rem;

}
</style>