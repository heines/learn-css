<template lang="pug">
  #app
    component(:is="isError")
    .p-menu
      .p-menu__btn(@click="transPage('buttonPage')") button
      .p-menu__btn(@click="transPage('drawPage')") draw
      .p-menu__btn(@click="transPage('labPage')") lab
      .p-menu__btn(@click="transPage('reportPage')") report
      .p-menu__btn(@click="openErrorPage('errorPage')") error
    h2 {{ currentTitle }}
    component(:is="current")
</template>

<script>
  import buttonPage from './pages/buttonPage';
  import reportPage from './pages/reportPage';
  import labPage from './pages/labPage';
  import errorPage from './pages/errorPage';
  import drawPage from './pages/drawPage';


  export default {
    name: 'App',
    components: {
      buttonPage,
      reportPage,
      labPage,
      drawPage,
      errorPage,
    },
    data: function() {
      return {
        current: 'buttonPage',
        isError: '',
        currentTitle: "buttonPage"
      }
    },
    methods: {
      transPage : function(page){
    		this.current = page;
        this.currentTitle = page;
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
  @import 'css/_variables.scss';

  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }

  h1, h2 {
    font-weight: normal;
  }

  .p-menu {
    display: flex;
    justify-content: center;
  }

  .p-menu__btn {
    height: 2em;
    width: 70px;
    display: inline-block;
    transition: .5s ease;
    border-bottom: 4px solid transparent;
    &:hover {
      border-bottom: 4px solid $midnight;
    }
  }
</style>
