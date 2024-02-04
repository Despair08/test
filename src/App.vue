<template>
  <div id="app">
    <Header>
    </Header>
    <Content></Content>
  </div>
</template>

<script>
import Header from './components/Header';
import Content from "./components/Content";


export default {
  name: 'App',
  components: {
    Header,
    Content,
  }
}
</script>

<style lang="scss">
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

html,
body {
  height: 100%;
  padding: 0;
  margin: 0;
}

img {
  display: block;
}

li {
  list-style: none;
}



#app {
  display: flex;
  flex-direction: column;
  min-height: 100%;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
