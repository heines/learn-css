<template lang="pug">
  div
    report1104
    aboutPosition
    report1103
    halo
    flexBox
</template>

<script>
  import flexBox from './flexBox1';
  import halo from './halo1';
  import aboutPosition from './aboutPosition';
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
      aboutPosition,
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
