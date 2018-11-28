<template lang="pug">
  .p-large-text-field
    p.p-large-text-field__text
      |Background text.
</template>

<script>
export default {
  name: 'bgText',
  data () {
    return {
    }
  }
}
</script>

<style lang="scss" scoped>
  .p-large-text-field {
    position: absolute;
    left: -10px;
    bottom: -10px;
    color: transparent;
    font-size: 5em;
    text-shadow: 0 0 15px gray;
    z-index: -1;
  }
</style>
