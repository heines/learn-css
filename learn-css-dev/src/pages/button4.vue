<template lang="pug">
  .base-box
    .contents__large
      .contents-section__row
        a(href="").c-btn.p-middle-btn 上に戻る
        a(href="").c-btn.p-small-btn 上
        a(href="").c-btn.p-triangle-btn 上
      .contents-section__row
        a(href="").c-btn.p-middle-cross-btn 上に戻る
      .contents-section__row
        a(href="").c-btn.p-middle-bar-btn 上に戻る
      .contents-section--bgcolor
        .box__inner-line
          .box__img__outer
            img(src='../assets/flower.jpg')
          p.box__p Photo by Anita Austvika on Unsplash
      .contents-section__row
        a(href="").c-btn.p-shadow-btn 影付き
        a(href="").c-btn.p-shutter-btn シャッター
      .contents-section__row
        a(href="").c-btn.p-camera-btn シャッター2
        a(href="").c-btn.p-btn--camera2 シャッター3
      .contents-section__row
        a(href="").c-btn.p-btn--camera3 シャッター4
      .contents-section__row
        p 星を描いたが汚い。
        .star
          .star__1
          .star__2
      .contents-section__row
        p
          |ポップアップブロックはclickイベントにすることで回避できる。
          br
          |clickイベントで『直接』操作するのが肝要。
          br
          |promiseとか途中でかますとブロックに引っかかる。
        lineShare
      .contents-section__row
        a.c-btn.p-btn--bgimage(href="https://heines.github.io/learn-css/")
      .contents-section__row
        p 画像が見えないのはurl()の解釈が実際と異なるのが原因。
        a.c-btn.p-btn--tagImage(href="https://heines.github.io/learn-css/")
          |パスを変える必要性。
      .contents-section__row
        a.c-btn.p-biscuit(href='')
          |オレオ
          br
          |食べたい
        p 外側はshadowで実装
      .contents-section__row
        a.c-btn.p-cookie(href='')
          |クッキー
      .contents-section__row
        .p-bite
          |はらへ
</template>

<script>
  import lineShare from '../components/lineShare';
  export default {
    name: 'button4',
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
  @import '../css/Layout/_layout.scss';
  .contents-section--bgcolor {
    position: relative;
    height: 200px;
    width: 300px;
    margin: 20px auto;
    padding: 8px;
    background-color: midnightblue;
  }

  .box__inner-line {
    height: 100%;
    border: 1px dashed white;
  }

  .box__p {
    width: 90%;
    display: block;
    color: white;
    border-bottom: 5px solid rgb(56, 56 ,255);
  }
  .box__img__outer {
    height: 100px;
    width: 150px;
    position: relative;
    margin: 10px;
    border-radius: 20px;
    background-color: white;
    & > img {
      height: 100%;
      border-radius: 20px;
      opacity: 0.5;
      &:hover {
        opacity: 1;
      }
    }
  }

.star {
  position: relative;
  width: 74px;
  margin-top: 45px;
  box-sizing: content-box;
  border-width: 69px 23px 0;
  border-style: solid;
  border-color: midnightblue transparent;
  &::before {
    content: "";
    position: absolute;
    height: 0;
    width: 0;
    top: -111px;
    left: -22px;
    border-width: 0 59px 42px;
    border-style: solid;
    border-color: transparent transparent midnightblue;
  }
  &::after {
    width: 0;
    height: 0;
    position: absolute;
    bottom: 0;
    left: 0;
    content: '';
    border-bottom: 10px solid white;
    border-top: 10px solid transparent;
    border-left: 37px solid transparent;
    border-right: 37px solid transparent;
  }
  &__1 {
    width: 100%;
    height: 100%;
    position: absolute;
    bottom: 0;
    left: 0;
    background-color: transparent;
    &::before {
      width: 0;
      height: 0;
      position: absolute;
      bottom: 72px;
      left: 24px;
      content: '';
      border-bottom: 10px solid transparent;
      border-top: 10px solid white;
      border-left: 37px solid transparent;
      border-right: 37px solid transparent;
      transform: rotate(36deg);
    }
    &::after {
      width: 0;
      height: 0;
      position: absolute;
      bottom: -10px;
      left: -10px;
      content: '';
      border-bottom: 10px solid transparent;
      border-top: 10px solid white;
      border-left: 37px solid transparent;
      border-right: 37px solid transparent;
      transform-origin: right;
      transform: rotate(108deg);
    }
  }
  &__2 {
    width: 100%;
    height: 100%;
    position: absolute;
    bottom: 0;
    left: 0;
    background-color: transparent;
    &::before {
      width: 0;
      height: 0;
      position: absolute;
      bottom: 72px;
      left: -24px;
      content: '';
      border-bottom: 10px solid white;
      border-top: 10px solid transparent;
      border-left: 37px solid transparent;
      border-right: 37px solid transparent;
      transform: rotate(144deg);
    }
    &::after {
      width: 0;
      height: 0;
      position: absolute;
      bottom: -10px;
      left: -64px;
      content: '';
      border-bottom: 10px solid white;
      border-top: 10px solid transparent;
      border-left: 37px solid transparent;
      border-right: 37px solid transparent;
      transform-origin: right;
      transform: rotate(72deg);
    }
  }
}

</style>
