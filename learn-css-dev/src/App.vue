<template lang="pug">
  #app
    component(:is="isError")
    div.menu
      div.menu__btn(@click="transPage('reportPage')") report
      div.menu__btn(@click="transPage('componentsPage')") home
      div.menu__btn(@click="openErrorPage('errorPage')") error
    component(:is="current")
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
  	},
    closeErrorPage : function(){
  		this.isError = '';
  	}
  }
}
</script>

<style lang="scss" scoped>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
menu {
  display: flex;
  justify-content: center;
}

.menu__btn {
  height: 2em;
  width: 50px;
  display: inline-block;
  transition: .5s ease;
  border-bottom: 4px solid transparent;
  &:hover {
    border-bottom: 4px solid midnightblue;
  }
}
</style>
