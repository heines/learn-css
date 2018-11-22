<template lang="pug">
  .hello
    naviber
    h1 Learn CSS
    div
      button1
      button2
      button3
      button4
      graph
</template>

<script>
  import flexBox from './flexBox1';
  import halo from './halo1';
  import balloon from './balloon';
  import aboutPosition from './aboutPosition';
  import button1 from './button1';
  import button2 from './button2';
  import button3 from './button3';
  import naviber from '../components/naviber';
  import report1103 from './report1103';
  import button4 from './button4';
  import graph from '../components/graph';
  export default {
    name: 'componentsPage',
    data () {
      return {
      };
    },
    components: {
      flexBox,
      halo,
      balloon,
      aboutPosition,
      button1,
      button2,
      button3,
      naviber,
      report1103,
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
