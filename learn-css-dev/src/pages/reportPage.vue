<template lang="pug">
  div
    h2 report
    div
      report1104
      aboutPosition
      report1103
      balloon
      halo
      flexBox
</template>

<script>
  import flexBox from './flexBox1';
  import halo from './halo1';
  import balloon from './balloon';
  import aboutPosition from './aboutPosition';
  import naviber from '../components/naviber';
  import report1103 from './report1103';
  import report1104 from './report1104';
  export default {
    name: 'reportPage',
    data () {
      return {
      };
    },
    components: {
      flexBox,
      halo,
      balloon,
      aboutPosition,
      naviber,
      report1103,
      report1104
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
  h1, h2 {
    font-weight: normal;
  }
</style>
