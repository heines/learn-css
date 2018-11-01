<template lang="pug">
  .hamb-flame
    .hamb-bar-1
    .hamb-bar-2
    .hamb-bar-3
</template>

<script>

export default {
  name: 'hamburger',
  data () {
    return {
    }
  }
}
</script>

<style lang="scss" scoped>
  .hamb-flame {
      width: 100px;
      height: 100px;
      align-items: center;
      position: relative;
      border: 1px solid #FAFAFA;
      background-color: #FAFAFA;
      box-sizing: border-box;
      border-radius: 20px;
      cursor:pointer;
      &:hover {
        background-color: white;
        transition: .8s ease-out;
        .hamb-bar {
          &-1 {
            position: absolute;
            top: 50%;
            transform: rotate(45deg);
          }
          &-2 {
            opacity: 0;
          }
          &-3 {
            position: absolute;
            top: 50%;
            transform: rotate(-45deg);
          }
        }
      }
  }

  .hamb-bar {
    &-1, &-2, &-3 {
      width: 60px;
      height: 5px;
      position: absolute;
      background-color: #CCCCCC;
      border-radius: 2px;
      transition: .8s ease-out;
    }
    &-1 {
      top: 30%;
      left: 20%;
    }
    &-2 {
      top: 50%;
      left: 20%;
    }
    &-3 {
      top:70%;
      left: 20%;
    }
  }

</style>
