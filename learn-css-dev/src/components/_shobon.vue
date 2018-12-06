<template lang="pug">
  .p-shobon
    .p-shobon__contours
      .p-shobon__hand--left
      .p-shobon__hand--right
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
  .p-shobon {
    padding-left: 20px;
    &__contours {
      width: 180px;
      height: 130px;
      position: relative;
      border-top-left-radius: 100px 80px;
      border-top-right-radius: 100px 80px;
      border-bottom-left-radius: 90px 60px;
      border-bottom-right-radius: 90px 60px;
      border: gray solid 1px;
      background-color: white;
    }
    &__hand--left {
      width: 30px;
      height: 20px;
      position: absolute;
      bottom: 10px;
      left: -10px;
      border-top-left-radius: 30px 15px;
      border-bottom-left-radius: 10px 10px;
      border-bottom-right-radius: 30px 10px;
      border: gray solid 1px;
      z-index: -1;
    }
    &__hand--right {
      width: 30px;
      height: 20px;
      position: absolute;
      bottom: 10px;
      right: -10px;
      border-top-right-radius: 30px 15px;
      border-bottom-right-radius: 10px 10px;
      border-bottom-left-radius: 30px 10px;
      border: gray solid 1px;
      z-index: -1;
    }
  }
</style>
