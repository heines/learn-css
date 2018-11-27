<template lang="pug">
  .p-ripple
</template>

<script>

export default {
  name: 'ripple',
  data () {
    return {
    }
  }
}
</script>

<style lang="scss" scoped>
  @import '../css/_variables.scss';
  .p-ripple {
    width: 200px;
    height: 200px;
    position: relative;
    background: radial-gradient(circle, lightblue, white, white, white);
    box-sizing: border-box;
    border-radius: 150px;
    transition: 3s ease-out;
    cursor: crosshair;
    opacity: 0;
    &:hover {
      opacity: 1;
    }
  }
</style>
