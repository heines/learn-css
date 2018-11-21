<template lang="pug">
  .c-marker
    .c-marker__background
    .c-marker__tag
      .c-marker__line
      .c-marker__element
</template>

<script>
export default {
  name: 'marker',
  data () {
    return {
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
      &:hover {
        background-color: #b3b3ff;
        box-sizing: border-box;
        box-shadow: 0 0 30px #ccccff;
        cursor: pointer;
      }
      &:active {
        bottom: 44px;
        // .c-marker__background{
        //   background-color: transparentize(black, 0.5);
        // } //子から親はjavascriptで変える。
      }
    }
  }
</style>
