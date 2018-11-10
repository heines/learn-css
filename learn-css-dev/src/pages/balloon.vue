<template lang="pug">
  .base-box
    .contents
      .box
        span.tooltip.top(aria-label="balloon")
          | text hover show tooltip bottom
    .elements-desc
      dl
        dt content: attr();
          dd 関数。指定の要素の属性の値を受け取り、スタイルシート内で使用できる。
        dt z-index
          dd 値が大きいほど前面に配置される。
</template>

<script>
  export default {
    name: 'baloon',
    data () {
      return {
      }
    }
  }
</script>

<style lang="scss" scoped>
  @import "../css/balloon.scss";
  @import "../css/Layout/_layout.scss"
</style>
