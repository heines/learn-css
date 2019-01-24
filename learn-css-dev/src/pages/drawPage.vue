<template lang="pug">
  div
    star
    graph
    .p-slide-show
      |test
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
  @import '../css/Object/Project/_slide-show.scss';
  h1, h2 {
    font-weight: normal;
  }
</style>
