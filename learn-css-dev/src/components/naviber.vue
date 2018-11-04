<template lang="pug">
  .naviber
    .naviber-contents
      a(href="#").naviber_a test1
    .naviber-contents
      a(href="#").naviber_a test2
    .naviber-contents
      a(href="#").naviber_a test3
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

  .naviber {
    height: 50px;
    display: flex;
    justify-content:space-around;
    flex-direction: row;
    position: sticky;
    top: 0;
    background-color: rgba(250, 250, 250, 0.5);
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
      color: rgba(250, 250, 250, 0.5);
      transition: 1s ease;
    }
    &:hover {
      box-sizing: border-box;
      background-color: rgba(250, 250, 250, 1.0);
      .naviber_a {
        color: $azureblue;
      }
    }
  }
</style>
