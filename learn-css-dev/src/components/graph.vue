<template lang="pug">
  .c-graph
    .c-graph__half
</template>

<script>

export default {
  name: 'shobon',
  data () {
    return {
    }
  }
}
</script>

<style lang="scss" scoped>
  @import '../css/_variables.scss';
  .c-graph {
    width: 100px;
    height: 100px;
    position: relative;
    background-color: gray;
    border-radius: 50px;
    &::before {
      width: 60px;
      height: 60px;
      display: block;
      position: absolute;
      bottom: 50%;
      left: 50%;
      content: '';
      background-color: white;
      border-radius: 0 60px 0 0;
      transform: rotate(0deg);
      transform-origin: left bottom;
      transition-duration: .6s;
      transition-timing-function: linear;
      z-index: 1;
    }
    &::after {
      width: 60px;
      height: 60px;
      display: block;
      position: absolute;
      bottom: 50%;
      left: 50%;
      content: '';
      background-color: white;
      border-radius: 0 60px 0 0;
      z-index: 1;
    }
    &:hover {
      &::before {
        transform: rotate(180deg);
        transform-origin: left bottom;
      }
      .c-graph__half {
        background-color: white;
      }
    }
  }
  .c-graph__half {
    width: 60px;
    height: 60px;
    position: absolute;
    top: 50%;
    left: 50%;
    border-radius: 0 0 60px;
    background-color: transparent;
    transition-delay: .3s;
  }
</style>
