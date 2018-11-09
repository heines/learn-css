<template lang="pug">
  .base-box
    .contents__large
      .contents-section__row
        a(href="").c-btn.p-btn__mdl 上に戻る
        a(href="").c-btn.p-btn__sml 上
        a(href="").c-btn.p-btn__top 上
      .contents-section__row
        a(href="").c-btn.p-btn__cross 上に戻る
      .contents-section__row
        a(href="").c-btn.p-btn__bar 上に戻る
      .contents-section--bgcolor
        .box__inner-line
          .box__img__outer
            img(src='../assets/flower.jpg')
          p.box__p Photo by Anita Austvika on Unsplash
      .contents-section__row
        a(href="").c-btn.p-btn--shadow 影付き
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

.p-btn--shadow {
  height: 70px;
  width: 150px;
  background-color: #0060e6;
  border-radius: 10px;
  border-bottom: 4px solid midnightblue;
  color: midnightblue;
  font-size: 20px;
  text-decoration: none;
  font-weight: bold;
  text-shadow: 1px 1px 1px rgba(255, 255, 255, 0.3);
  &:active {
    border-bottom: 0;
    border-top: 4px solid transparent;
  }
}
</style>
