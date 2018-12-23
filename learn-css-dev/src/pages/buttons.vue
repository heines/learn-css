<template lang="pug">
  .base-box
    .contents__large
      .c-flexbox
        a.c-btn.p-balloon.p-balloon__top(label="balloon" href="#")
          | text hover show balloon bottom
        a.p-btn-round(href="#")
      .c-flexbox
        a(href="").c-btn.p-btn-middle 上に戻る
        a(href="").c-btn.p-btn-small 上
        a(href="").c-btn.p-btn-triangle 上
        .p-btn-cross-middle__outer
          a(href="").c-btn.p-btn-cross-middle 上に戻る
        a(href="").c-btn.p-btn-bar-middle 上に戻る
      .c-flexbox
        a(href="").c-btn.p-btn-shadow 影付き
        a(href="").c-btn.p-btn-shutter シャッター
        a(href="").c-btn.p-btn-camera カメラ
        a(href="").c-btn.p-btn-camera2 カメラ2
        a(href="").c-btn.p-btn-camera3 カメラ3
      .c-flexbox
        .p-image-box
          .p-image-box__line
            .p-image-box__img
              img(src='../assets/flower.jpg')
            p.p-image-box__text Photo by Anita Austvika on Unsplash
      .c-flexbox
        a.c-btn.p-btn__bgimage(href="https://heines.github.io/learn-css/")
        a.c-btn.p-btn__tag-image(href="https://heines.github.io/learn-css/")
          |擬似要素に画像を追加
        lineShare
      .c-flexbox
        a.c-btn.p-btn-biscuit(href='')
          |オレオ
          br
          |食べたい
        a.c-btn.p-btn-cookie(href='')
          |クッキー
        .p-btn-bite__outer
          a.c-btn.p-btn-bite(href='https://heines.github.io/learn-css/')
            |はらへ
      .c-flexbox
        a.c-btn.p-btn-curtain(href='')
          |カーテン
        a.c-btn.p-btn-light(href='#')
          |光る
        a.c-btn.p-btn-light-white 色が逆
      .c-flexbox
        a.c-btn.p-btn-blur(href='')
          img(src='../assets/sky.jpg')
        a.c-btn.p-btn-blur-opacity(href='' tags='entrance') sky
          .p-btn-blur-opacity__bg1
          .p-btn-blur-opacity__bg2
        a.c-btn.p-btn-fill(href='#' data-text='testtest') testtest
      .c-flexbox
        a.c-btn.p-btn-underline
          |下線を引く1。文章は長めの方がいいか
        a.c-btn.p-btn-underline.p-btn-underline--center
          |下線を引く2
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
  @import '../css/Object/Project/_btn-cross-middle.scss';
  @import '../css/Object/Project/_btn-curtain.scss';
  @import '../css/Object/Project/_btn-blur.scss';
  @import '../css/Object/Project/_balloon.scss';
  @import '../css/Object/Project/_image-box.scss';
  @import '../css/Object/Project/_btn-biscuit.scss';
  @import '../css/Object/Project/_cookie.scss';
  @import '../css/Object/Project/_btn-fill.scss';
  @import '../css/Object/Project/_btn-light.scss';
  @import '../css/Object/Project/_btn-underline.scss';
  @import '../css/Layout/_layout.scss';
</style>
