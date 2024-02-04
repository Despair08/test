<template>
  <nav class="header">
    <div class="container">
      <Button></Button>
    </div>
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
  padding: 0 20px;
  background-color: #42b983;
  width: 100%;
}
</style>