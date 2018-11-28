<template lang="pug">
  div
    h2 draw
    star
    graph
</template>

<script>
  import star from '../components/star';
  import graph from '../components/graph';

  export default {
    name: 'drawPage',
    data () {
      return {
      };
    },
    components: {
      star,
      graph
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
  h1, h2 {
    font-weight: normal;
  }
</style>
