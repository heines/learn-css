<template lang="pug">
  .base-box
    .contents__large
      .contents-section__row
        span.p-tooltip.p-tooltip__top(aria-label="balloon")
          | text hover show tooltip bottom
      .contents-section__row
        a.button_a(href="#")
      .contents-section__row
        a(href="").c-btn.p-middle-btn 上に戻る
        a(href="").c-btn.p-small-btn 上
        a(href="").c-btn.p-triangle-btn 上
        a(href="").c-btn.p-middle-cross-btn 上に戻る
        a(href="").c-btn.p-middle-bar-btn 上に戻る
      .contents-section__row
        a(href="").c-btn.p-shadow-btn 影付き
        a(href="").c-btn.p-shutter-btn シャッター
        a(href="").c-btn.p-camera-btn シャッター2
        a(href="").c-btn.p-btn--camera2 シャッター3
        a(href="").c-btn.p-btn--camera3 シャッター4
      .contents-section__row
        .p-image-box
          .p-image-box__inner-line
            .p-image-box__img__outer
              img(src='../assets/flower.jpg')
            p.p-image-box__text Photo by Anita Austvika on Unsplash
      .contents-section__row
        a.c-btn.p-btn--bgimage(href="https://heines.github.io/learn-css/")
        a.c-btn.p-btn--tagImage(href="https://heines.github.io/learn-css/")
          |パスを変える必要性。
        lineShare
      .contents-section__row
        a.c-btn.p-biscuit(href='')
          |オレオ
          br
          |食べたい
        a.c-btn.p-cookie(href='')
          |クッキー
        .p-bite
          |はらへ
</template>

<script>
  import lineShare from '../components/lineShare';
  export default {
    name: 'buttons',
    data () {
      return {
      }
    },
    components: {
      lineShare
    }
  }
</script>

<style lang="scss" scoped>
  @import '../css/Object/Component/_btn.scss';
  @import '../css/Object/Project/_btn.scss';
  @import "../css/Object/Project/_balloon.scss";
  @import "../css/Object/Project/_image-box.scss";
  @import '../css/Layout/_layout.scss';
</style>
