<template lang="pug">
  div.hello
    h1 Learn CSS
    div
      flexBox
</template>

<script>
import flexBox from './flexBox1';
export default {
  name: 'HelloCSS',
  data () {
    return {
    };
  },
  components: {
    flexBox
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
h1, h2 {
  font-weight: normal;
}
</style>
