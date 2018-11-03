<template>
  <div id="app">
    <HelloCSS />
  </div>
</template>

<script>
import HelloCSS from './pages/HelloCSS'

export default {
  name: 'App',
  components: {
    HelloCSS
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
