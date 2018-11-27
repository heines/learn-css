<template lang="pug">
  .hello
    naviber
    h1 Learn CSS
    button1
    hamburger
    button3
    button4
    graph
</template>

<script>
  import button1 from './button1';
  import button3 from './button3';
  import hamburger from '../components/hamburger';
  import naviber from '../components/naviber';
  import button4 from './button4';
  import graph from '../components/graph';
  export default {
    name: 'componentsPage',
    data () {
      return {
      };
    },
    components: {
      button1,
      hamburger,
      button3,
      naviber,
      button4,
      graph,
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
  h1, h2 {
    font-weight: normal;
  }
</style>
