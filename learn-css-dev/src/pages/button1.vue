<template lang="pug">
  .base-box
    .contents
      .contents-section
        a.button_a(href="#")
      .contents-section
        .tab-menu
          a.tab-menu__a(href="#") 1
          a.tab-menu__b(href="#") 2
          a.tab-menu__a(href="#") 3
</template>

<script>
  export default {
    name: 'button1',
    data () {
      return {
      }
    }
  }
</script>

<style lang="scss" scoped>
  @import '../css/Layout/_layout.scss';
  @import '../css/Object/Project/_tab.scss';
  @import '../css/Object/Project/_btn.scss';
  .contents {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 500px;
    height: 200px;
    padding: 50px;
  }

  .contents-section {
    margin: 10px 0;
  }
</style>
