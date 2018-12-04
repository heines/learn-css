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
  @import '../css/_variables.scss';
  .p-marker {
    &__tag {
      width: 50px;
      height: 50vh;
      position: absolute;
      top: 0;
      right: 12px;
    }
    &__line {
      width: 1px;
      height: calc(50vh - 50px);
      position: absolute;
      top: 0;
      right: 12px;
      background-color: $midnight;
    }
    &__background {
      position: fixed;
      width: 100vw;
      height: 100vh;
      background-color: transparent;
      &.active {
        background-color: transparentize(black, 0.5);
        z-index: 2;
      }
    }
    &__element {
      width: 24px;
      height: 24px;
      position: absolute;
      bottom: 50px;
      right: 0;
      border-radius: 13px;
      background-color: $midnight;
      transition: .5s ease;
      z-index:3;
      &.rise {
        background-color: #b3b3ff;
      }
      &:hover {
        background-color: #b3b3ff;
        box-sizing: border-box;
        box-shadow: 0 0 30px #ccccff;
        cursor: pointer;
      }
      &:active {
        bottom: 44px;
      }
    }
  }
</style>
