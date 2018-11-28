<template lang="pug">
  #app
    component(:is="isError")
    .menu
      .menu__btn(@click="transPage('reportPage')") report
      .menu__btn(@click="transPage('componentsPage')") button
      .menu__btn(@click="transPage('drawPage')") draw
      .menu__btn(@click="transPage('laboPage')") labo
      .menu__btn(@click="transPage('bgImages')") bg
      .menu__btn(@click="openErrorPage('errorPage')") error
    component(:is="current")
</template>

<script>
import componentsPage from './pages/componentsPage';
import reportPage from './pages/reportPage';
import laboPage from './pages/laboPage';
import errorPage from './pages/errorPage';
import drawPage from './pages/drawPage';
import bgImages from './pages/bgimages';


export default {
  name: 'App',
  components: {
    componentsPage,
    reportPage,
    laboPage,
    drawPage,
    bgImages,
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
  width: 70px;
  display: inline-block;
  transition: .5s ease;
  border-bottom: 4px solid transparent;
  &:hover {
    border-bottom: 4px solid midnightblue;
  }
}
</style>
