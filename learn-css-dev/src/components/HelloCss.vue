<template lang="pug">
  div.hello
    h1 Learn CSS
    div
      flexBox
      halo
      balloon
      aboutPosition
      button1
</template>

<script>
import flexBox from './flexBox1';
import halo from './halo1';
import balloon from './balloon';
import aboutPosition from './aboutPosition';
import button1 from './button1';
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
    button1
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
h1, h2 {
  font-weight: normal;
}
</style>
