<template lang="pug">
  .c-marker
    .c-marker__background(:class='{active: isActive}')
    .c-marker__tag
      .c-marker__line
      .c-marker__element(@mouseup='braided')
</template>

<script>
  export default {
    name: 'lightSwitch',
    data () {
      return {
        isActive: false
      }
    },
    methods: {
      braided: function() {
        (this.isActive === true ? this.isActive = false : this.isActive = true);
      }
    }
  }
</script>

<style lang="scss" scoped>
  .c-marker {
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
      background-color: midnightblue;
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
      background-color: midnightblue;
      transition: .5s ease;
      z-index:3;
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
