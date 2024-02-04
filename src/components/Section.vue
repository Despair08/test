<template>
  <section class="content__section">
    <h1 class="section__header">Блок с контентом</h1>
    <Article__oneVue></Article__oneVue>
    <Article__two></Article__two>
    <Article__three></Article__three>
    <Article__four></Article__four>
  </section>
</template>

<script>
import Article__oneVue from './Article__one.vue';
import Article__two from './Article__two.vue';
import Article__three from './Article__three.vue';
import Article__four from './Article__four.vue';
export default {
  name: 'content-section',
  components: {
    Article__oneVue,
    Article__two,
    Article__three,
    Article__four,
  }
}
</script>

<style>
.content__section {
  display: flex;
  flex-direction: column;
  row-gap: 20px;
}

.section__header {
  padding: 20px 0 0 0;
}
</style>