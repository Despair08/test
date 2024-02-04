<template>
  <nav class="header">
    <Button></Button>
  </nav>
</template>

<script>
import Button from './Button.vue';

export default {
  name: 'app-header',
  components: {
    Button,
  }
}
</script>

<style>
.header {
  display: block;
  align-items: center;
  height: 50px;
  padding: 0 20px;
  background-color: #42b983;
}
</style>