<template lang="pug">
  .tab-menu
    a.tab-menu__a(href="#") 1
    a.tab-menu__b(href="#") 2
    a.tab-menu__a(href="#") 3
</template>

<script>
  export default {
    name: 'tab',
    data () {
      return {
      }
    }
  }
</script>

<style lang="scss" scoped>
  @import '../css/Object/Project/_tab.scss';
</style>
