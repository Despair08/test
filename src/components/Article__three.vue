<template>
  <article class="block__three">
    <h2 class="three__header">Lorem ipsum dolor sit amet.</h2>
    <input v-model="message" class="three__input" placeholder="Введите текст">
    <p class="three__text">Текст: {{ message }}</p>

  </article>
</template>

<script>
export default {
  name: 'article-three',
  data: function () {
    return {
      message: ''
    };
  }
}
</script>

<style>
.block__three {
  display: flex;
  flex-direction: column;
  row-gap: 20px;
}

.three__input {
  max-width: 400px;
  height: 20px;
  font-size: 18px;
}
</style>