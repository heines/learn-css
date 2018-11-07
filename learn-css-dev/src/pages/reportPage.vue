<template lang="pug">
  div
    naviber
    h2 report
    div
      flexBox
      halo
      balloon
      aboutPosition
</template>

<script>
import flexBox from './flexBox1';
import halo from './halo1';
import balloon from './balloon';
import aboutPosition from './aboutPosition';
import naviber from '../components/naviber';
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
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
h1, h2 {
  font-weight: normal;
}
</style>
