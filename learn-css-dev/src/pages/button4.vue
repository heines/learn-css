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
        a(href="").c-btn.p-btn--shutter
          span シャッター
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

.p-btn--shutter {
  width: 150px;
  position: relative;
  background-color: midnightblue;
  color: white;
  font-weight: bold;
  border-radius: 10px;
}

.p-btn--shutter span {
  width: 100%;
  height: 100%;
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  color: midnightblue;
  z-index: 1;
  &:hover {
    color: white;
  }
}

.p-btn--shutter::before,
.p-btn--shutter::after {
  width: 50%;
  height: 100%;
  position: absolute;
  top: 0;
  content: "";
  display: block;
  color: midnightblue;
  background-color: #FFF;
  transition: .5s;
}
.p-btn--shutter::before {
  left: 0;
}
.p-btn--shutter::after {
  right: 0;
}

.p-btn--shutter:hover:before,
.p-btn--shutter:hover:after {
  width: 0;
  background-color: #FFF;
}
</style>
