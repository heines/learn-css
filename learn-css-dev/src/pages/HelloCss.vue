<template lang="pug">
  div.hello
    naviber
    h1 Learn CSS
    div
      flexBox
      halo
      balloon
      aboutPosition
      button1
      button2
      button3
      report1103
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
export default {
  name: 'HelloCSS',
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
    report1103
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
h1, h2 {
  font-weight: normal;
}
</style>
