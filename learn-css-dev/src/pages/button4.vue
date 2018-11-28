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
        .contents-section--bgcolor
          .box__inner-line
            .box__img__outer
              img(src='../assets/flower.jpg')
            p.box__p Photo by Anita Austvika on Unsplash
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
  @import "../css/Object/Project/_balloon.scss";
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



</style>
