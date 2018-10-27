<template lang="pug">
  div.hello
    h1 Learn CSS
    div
      flexBox
      halo
</template>

<script>
import flexBox from './flexBox1';
import halo from './halo1';
export default {
  name: 'HelloCSS',
  data () {
    return {
    };
  },
  components: {
    flexBox,
    halo
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
h1, h2 {
  font-weight: normal;
}
</style>
