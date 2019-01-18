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
        a.c-btn.p-btn-curtain(href='')
          |カーテン
        a.c-btn.p-btn-light(href='#')
          |光る
        a.c-btn.p-btn-light-white(href='#') 色が逆
      .c-flexbox
        a.c-btn.p-btn-blur(href='')
          img(src='../assets/sky.jpg')
        a.c-btn.p-btn-blur-opacity(href='' tags='entrance') sky
          .p-btn-blur-opacity__bg1
          .p-btn-blur-opacity__bg2
        a.c-btn.p-btn-fill(href='#' data-text='testtest') testtest
      .c-flexbox
        a(href="").c-btn.p-btn-line-extend
          |線を引く1。文章は長めの方がいいか
        a(href="").c-btn.p-btn-line-extend.p-btn-line-extend--center
          |線を引く2。テストテキスト（modifier 中央から伸びる）
      .c-flexbox
        a(href="").c-btn.p-btn-line-extend.p-btn-line-extend__center
          |線を引く3。テストテキスト（element 中央に線が置かれる）
        a(href="").c-btn.p-btn-line-extend.p-btn-line-extend__center.p-btn-line-extend--center
          |線を引く4。テストテキスト（modifier 中央から伸びる）
      .c-flexbox
        a(href="").c-btn.p-btn-offset
          |テキストがオフセットする。
        a(href="").c-btn.p-btn-offset.p-btn-offset__mark
          |テキストがオフセットする。（マークつき）
      .c-flexbox
        a(href="").c-btn.p-btn-floats
          |テキストが浮かぶ。
        a(href="").c-btn.p-btn-floats.p-btn-floats__line
          |テキストが浮かぶ。（下線つき）
      .c-flexbox
        a(href="").c-btn.p-btn-spin
          |回
        a(href="").c-btn.p-btn-spin-string
          .p-btn-spin-string-char0 回
          .p-btn-spin-string-char1 っ
          .p-btn-spin-string-char2 て
          .p-btn-spin-string-char3 出
          .p-btn-spin-string-char4 て
          .p-btn-spin-string-char5 く
          .p-btn-spin-string-char6 る
        a(href="").c-btn.p-btn-fallen-string
          .p-btn-fallen-string-char0 落
          .p-btn-fallen-string-char1 ち
          .p-btn-fallen-string-char2 て
          .p-btn-fallen-string-char3 出
          .p-btn-fallen-string-char4 て
          .p-btn-fallen-string-char5 く
          .p-btn-fallen-string-char6 る
      .c-flexbox
        a(href="").c-btn.p-btn-slidein-string
          p.p-btn-slidein-string__text
            |slide in
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
        .c-scroll-arrow
          .c-scroll-arrow__box1
          .c-scroll-arrow__box2
          .c-scroll-arrow__box3
          .c-scroll-arrow__up
            .c-scroll-arrow__box1
            .c-scroll-arrow__box1
            .c-scroll-arrow__box1
          .c-scroll-arrow__down
            .c-scroll-arrow__box2
            .c-scroll-arrow__box2
            .c-scroll-arrow__box2
          .c-scroll-arrow__box3
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
  @import '../css/Object/Project/_btn-line-extend.scss';
  @import '../css/Object/Project/_btn-offset.scss';
  @import '../css/Object/Project/_btn-floats.scss';
  @import '../css/Object/Project/_btn-spin.scss';
  @import '../css/Object/Project/_btn-spin-string.scss';
  @import '../css/Object/Project/_btn-fallen-string.scss';
  @import '../css/Object/Project/_btn-slidein-string.scss';
  @import '../css/Layout/_layout.scss';

  .c-scroll-arrow {
    width: 50px;
    height: 150px;
    display: flex;
    flex-direction: column;
    align-items: center;
    &__box1, &__box2, &__box3 {
      width: 5px;
      height: 5px;
      margin-bottom: 1px;
      background-color: blue;
    }
    &__up {
      width: 30px;
      display: flex;
      justify-content: space-around;
    }
    &__down {
      width: 21px;
      display: flex;
      justify-content: space-around;
    }
  }
</style>
