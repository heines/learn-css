<template lang="pug">
  .hello
    markers
    h2 labo
    novel
    proverb
    graph
    graph
    graph
    graph
</template>

<script>
  import novel from '../components/novel';
  import proverb from '../components/proverb';
  import graph from '../components/graph';
  import shobon from '../components/shobon';
  import markers from '../components/marker';
  export default {
    name: 'componentsPage',
    data () {
      return {
      };
    },
    components: {
      novel,
      proverb,
      shobon,
      graph,
      markers
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
  h1, h2 {
    font-weight: normal;
  }
</style>
