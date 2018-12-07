<template lang="pug">
  .p-wave
    p.p-wave__text testpage
</template>

<script>
export default {
  name: 'wave'
}
</script>

<style lang="scss" scoped>
  .p-wave {
    width: 100vw;
    height: 110px;
    position: fixed;
    bottom: 0;
    left: 0;
    background-color: transparentize(#87cefa, 0.8);
    animation: floating 3s forwards 5s ease-in-out infinite;
    &__text {
      position: absolute;
      bottom: 0;
      right: 50px;
    }
  }

  @keyframes floating {
    0% {
      height: 110px;
    }
    50% {
      height: 130px;
    }
    100% {
      height: 110px;
    }
  }
</style>
