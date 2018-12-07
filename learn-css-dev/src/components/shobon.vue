<template lang="pug">
  .p-shobon
    a(href='#').c-btn
      img(src='../assets/shobon.svg')
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>
  .p-shobon {
    position: fixed;
    top: 0;
    right: 10px;
    width: 80px;
    height: 100vh;
    img {
      display: block;
      position: absolute;
      bottom: calc(100% - 100px);
      right: 0;
      animation-name: fallen;
      animation-timing-function: ease;
      animation-duration: 5s;
      animation-fill-mode: forwards;
    }
  }

  @keyframes fallen {
    0% {
      bottom: calc(100% - 100px);
      opacity: 0
    }
    50% {
      opacity: 1;
    }
    100% {
      bottom: 100px;
    }
  }
</style>
