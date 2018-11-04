<template lang="pug">
  .base-box
    h2.title 復習
    .date-box
      p.date-box_text 2018 Nov 4th
    .desc-box
      p.desc-box_text
        |ボタンを作る。
        br
        |FLOCSSに合わせてリファクタリングしようとしてるんだけど、なかなか難しい。
        br
        |とりあえずObjectフォルダを作ってみた。
    .contents__large
      .contents-section__row
        a(href="").c-btn.p-btn__mdl 上に戻る
        a(href="").c-btn.p-btn_sml 上
        a(href="").c-btn.p-btn_top 上
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
