<template>
  <article class="block__four">
    <h2 class="four__header">Lorem, ipsum.</h2>
    <div class="img__container">
      <img class="four__image" src="../assets/four.webp" alt="image four block">
    </div>
  </article>
</template>

<script>
export default {
  name: 'article-four',
}
</script>

<style>
.four__header {
  text-align: center;
  padding-bottom: 20px;
}

.img__container {
  position: relative;
  padding: 0 0 58% 0;
  overflow: hidden;
}

.four__image {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>