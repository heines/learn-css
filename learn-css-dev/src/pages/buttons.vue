<template lang="pug">
  .base-box
    .contents__large
      .c-flexbox
        a.c-btn.p-tooltip.p-tooltip__top(label="balloon" href="#")
          | text hover show tooltip bottom
        a.p-btn-round(href="#")
      .c-flexbox
        a(href="").c-btn.p-middle-btn 上に戻る
        a(href="").c-btn.p-small-btn 上
        a(href="").c-btn.p-triangle-btn 上
        .p-middle-cross-btn__outer
          a(href="").c-btn.p-middle-cross-btn 上に戻る
        a(href="").c-btn.p-middle-bar-btn 上に戻る
      .c-flexbox
        a(href="").c-btn.p-shadow-btn 影付き
        a(href="").c-btn.p-shutter-btn シャッター
        a(href="").c-btn.p-camera-btn シャッター2
        a(href="").c-btn.p-btn--camera2 シャッター3
        a(href="").c-btn.p-btn--camera3 シャッター4
      .c-flexbox
        .p-image-box
          .p-image-box__inner-line
            .p-image-box__img__outer
              img(src='../assets/flower.jpg')
            p.p-image-box__text Photo by Anita Austvika on Unsplash
      .c-flexbox
        a.c-btn.p-btn--bgimage(href="https://heines.github.io/learn-css/")
        a.c-btn.p-btn--tagImage(href="https://heines.github.io/learn-css/")
          |パスを変える必要性。
        lineShare
      .c-flexbox
        a.c-btn.p-biscuit(href='')
          |オレオ
          br
          |食べたい
        a.c-btn.p-cookie(href='')
          |クッキー
        .p-bite__outer
          a.c-btn.p-bite(href='https://heines.github.io/learn-css/')
            |はらへ
      .c-flexbox
        a.c-btn.p-btn-curtain(href='')
          |カーテン
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
  @import '../css/Object/Component/_flexbox.scss';
  @import '../css/Object/Project/_btn.scss';
  @import '../css/Object/Project/_btn-small.scss';
  @import '../css/Object/Project/_btn-curtain.scss';
  @import '../css/Object/Project/_balloon.scss';
  @import '../css/Object/Project/_image-box.scss';
  @import '../css/Object/Project/_cookie.scss';
  @import '../css/Layout/_layout.scss';
</style>
