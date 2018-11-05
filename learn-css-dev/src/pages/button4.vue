<template lang="pug">
  .base-box
    h2.title 復習
    .date-box
      p.date-box_text 2018 Nov 4th / 2018 Nov 5th
    .contents__large
      .contents-section__row
        a(href="").c-btn.p-btn__mdl 上に戻る
        a(href="").c-btn.p-btn__sml 上
        a(href="").c-btn.p-btn__top 上
      .contents-section__row
        a(href="").c-btn.p-btn__cross 上に戻る
      .contents-section__row
        a(href="").c-btn.p-btn__bar 上に戻る
</template>

<script>

export default {
  name: 'button4',
  data () {
    return {
    }
  }
}
</script>

<style lang="scss" scoped>
@import '../css/Object/Component/_btn.scss';
@import '../css/Object/Project/_btn__color.scss';
@import '../css/Layout/_layout.scss';

</style>
