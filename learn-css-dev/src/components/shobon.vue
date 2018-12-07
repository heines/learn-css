<template lang="pug">
  .p-shobon
    a(href='#').c-btn
      img(src='../assets/shobon.svg')
</template>

<script>
export default {
  name: 'shobon'
}
</script>

<style lang="scss" scoped>
  .p-shobon {
    position: fixed;
    top: 0;
    right: 10px;
    width: 100px;
    height: 100vh;
    img {
      width: 80px;
      height: auto;
      display: block;
      position: absolute;
      right: 0;
      bottom: calc(100% - 100px);
      animation:
        fallen 5s forwards cubic-bezier(.56, .11, 0, 1.18),
        floating 3s forwards 5.1s ease-in-out infinite;
      &:hover::after {
        width: 10px;
        height: 10px;
        position: absolute;
        left: 0;
        top: 0;
        background-color: blue;
      }
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

  @keyframes floating {
    0% {
      bottom: 100px;
    }
    50% {
      bottom: 110px;
    }
    100% {
      bottom: 100px;
    }
  }
</style>
