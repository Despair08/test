<template>
  <div class="container">
    <Section></Section>
  </div>
</template>

<script>
import Section from './Section.vue';
export default {
  name: 'app-content',
  components: {
    Section
  }
}
</script>

<style>
.contant__container {
  padding: 0 15px;
  flex-grow: 1;
}
</style>