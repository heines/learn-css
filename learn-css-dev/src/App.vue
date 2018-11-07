<template>
  <div id="app">
    <component :is="current" />
    <button @click="transPage('reportPage')">report</button>
    <button @click="transPage('componentsPage')">home</button>
    <button @click="openErrorPage('errorPage')">error test</button>
    <component :is="isError" />
  </div>
</template>

<script>
import componentsPage from './pages/componentsPage';
import reportPage from './pages/reportPage';
import errorPage from './pages/errorPage';

export default {
  name: 'App',
  components: {
    componentsPage,
    reportPage,
    errorPage
  },
  data: function() {
    return {
      current: 'componentsPage',
      isError: ''
    }
  },
  methods: {
    transPage : function(page){
  		this.current = page;
  	},
    openErrorPage : function(page){
  		this.isError = page;
  	}
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
