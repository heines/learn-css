<template lang="pug">
  .hello
    naviber
    tabmenu
    hamburger
    ripple
    buttons
</template>

<script>
  import tabmenu from '../components/tab-menu';
  import hamburger from '../components/hamburger';
  import naviber from '../components/naviber';
  import ripple from '../components/ripple';
  import buttons from './buttons';
  export default {
    name: 'buttonPage',
    data () {
      return {
      };
    },
    components: {
      hamburger,
      tabmenu,
      ripple,
      naviber,
      buttons,
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
  h1, h2 {
    font-weight: normal;
  }
</style>
