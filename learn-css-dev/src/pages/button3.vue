<template lang="pug">
  .base-box
    .contents
      .contents-section
        ripple
</template>

<script>
  import ripple from '../components/ripple';
  export default {
    name: 'button3',
    components: {
      ripple
    }
  }
</script>

<style lang="scss" scoped>
  @import "../css/Layout/_layout.scss"
</style>
