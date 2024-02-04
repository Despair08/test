<template>
  <div class="contant__container">
    {{ text }}
  </div>
</template>

<script>
export default {
  name: 'app-content',
  data() {
    return {
      text: 'content'
    }
  }
}
</script>

<style>
.contant__container {
  max-width: 95%;
  margin: 0 auto;
  flex-grow: 1;
}
</style>