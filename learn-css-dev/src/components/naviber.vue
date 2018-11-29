<template lang="pug">
  .p-naviber
    .p-naviber-contents
      a.p-naviber_a(href="#") test1
    .p-naviber-contents
      a.p-naviber_a(href="#") test2
    .p-naviber-contents
      a.p-naviber_a(href="#") test3
</template>

<script>
export default {
  name: 'naviber',
  data () {
    return {
    }
  }
}
</script>

<style lang="scss" scoped>
@import '../css/_variables';
  .p-naviber {
    height: 50px;
    display: flex;
    justify-content:space-around;
    flex-direction: row;
    position: sticky;
    top: 0;
    border-bottom: 1px solid rgba(250, 250, 250, 0.5);
    transition: 1s ease;
    &-contents {
      display: flex;
      justify-content: center;
      align-items: center;
    }
    &_a {
      display: block;
      text-decoration: none;
      font-size: 1.5em;
      color: transparent;
      transition: 1s ease;
    }
    &:hover {
      box-sizing: border-box;
      background-color: rgba(250, 250, 250, 1.0);
      .p-naviber_a {
        color: blue;
      }
    }
  }
</style>
