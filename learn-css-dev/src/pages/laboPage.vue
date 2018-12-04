<template lang="pug">
  .hello
    lightSwitch
    novel
    proverb
    manuscript
    frosted
    bgText
</template>

<script>
  import novel from '../components/novel';
  import proverb from '../components/proverb';
  import shobon from '../components/shobon';
  import lightSwitch from '../components/lightSwitch';
  import bgText from '../components/bgText';
  import manuscript from '../components/manuscript';
  import frosted from '../components/frosted';

  export default {
    name: 'componentsPage',
    data () {
      return {
      };
    },
    components: {
      novel,
      proverb,
      manuscript,
      shobon,
      lightSwitch,
      bgText,
      frosted
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
  h1, h2 {
    font-weight: normal;
  }
</style>
