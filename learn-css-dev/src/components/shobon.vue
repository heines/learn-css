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
      top: 0;
      right: 0;
      animation-name: fallen;
      animation-timing-function: ease;
      animation-duration: 5s;
      animation-fill-mode: forwards;
    }
  }

  @keyframes fallen {
    0% {
      top: 0;
      opacity: 0
    }
    50% {
      opacity: 1;
    }
    100% {
      top: 90%;
    }
  }
</style>
