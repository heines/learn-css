<template lang="pug">
  .p-marker
    .p-marker__background(:class='{active: isBraided}')
    .p-marker__tag
      .p-marker__line
      .p-marker__element(:class='{rise: isBraided}' @mouseup='braided')
</template>

<script>
  export default {
    name: 'lightSwitch',
    data () {
      return {
        isBraided: false
      }
    },
    methods: {
      braided: function() {
        (this.isBraided === true ? this.isBraided = false : this.isBraided = true);
      }
    }
  }
</script>

<style lang="scss" scoped>
  @import '../css/Object/Project/_marker.scss';
</style>
