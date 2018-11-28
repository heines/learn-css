<template lang="pug">
  .hello
    naviber
    h1 Learn CSS
    tabmenu
    hamburger
    ripple
    button4
</template>

<script>
  import tabmenu from '../components/tab-menu';
  import hamburger from '../components/hamburger';
  import naviber from '../components/naviber';
  import ripple from '../components/ripple';
  import button4 from './button4';
  export default {
    name: 'componentsPage',
    data () {
      return {
      };
    },
    components: {
      hamburger,
      tabmenu,
      ripple,
      naviber,
      button4,
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
  h1, h2 {
    font-weight: normal;
  }
</style>
