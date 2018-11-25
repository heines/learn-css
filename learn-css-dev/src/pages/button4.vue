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
        a(href="").c-btn.p-btn--shutter シャッター
      .contents-section__row
        a(href="").c-btn.p-btn--camera シャッター2
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
        p スマホからだと背景画像が見えない。なんでだろう。
        a.p-btn--bgimage(href="https://heines.github.io/learn-css/")
      .contents-section__row
        p
          |url()の解釈が実際と異なるのが原因。相対パスでやりたいけど無理か。
          br
          |方法は別途考える。どうしてたっけ
        a.p-btn--tagImage(href="https://heines.github.io/learn-css/")
          |パスを変える必要性。
      .contents-section__row
        a.p-btn__biscuit(href='')
          |オレオ
          br
          |食べたい
        p 外側はshadowで実装
      .contents-section__row
        a.p-btn__cookie(href='')
          |クッキー
      .contents-section__row
        .p-btn__bite
          |改良の余地あり
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
  height: 50px;
  position: relative;
  color: midnightblue;
  font-weight: bold;
  border-radius: 10px;
  overflow: hidden;
  &:hover {
    color: white;
  }
}

.p-btn--shutter::before {
  width: 100%;
  height: 100%;
  position: absolute;
  top: 0;
  content: '';
  display: block;
  z-index: -1;
  background-color: midnightblue;
  transition: .2s;
  transform: scale(0, 1);
}

.p-btn--shutter:hover:before {
  transform: scale(1, 1);
}

.p-btn--camera {
  width: 150px;
  height: 50px;
  display: flex;
  position: relative;
  color: midnightblue;
  font-weight: bold;
  text-decoration: none;
  border: 2px solid midnightblue;
  box-sizing: border-box;
  transition: .2s;
  overflow: hidden; // はみ出た平行四辺形をhiddenする
}

.p-btn--camera:hover {
  color: white;
}

.p-btn--camera::before { // 平行四辺形を乗せているだけ。
  width: 120%; // ベースの四角を覆えればいい大きさ
  height: 100%;
  position: absolute;
  top: 0;
  left: -10%;
  z-index: -1;
  content: '';
  background: midnightblue;
  transform: skewX(-30deg) scale(0, 1); // 傾き。scaleはノルム
  transition: transform .2s;
}
.p-btn--camera:hover::before {
  transform: skewX(-30deg) scale(1, 1);
}

.p-btn--camera2 {
  width: 150px;
  height: 50px;
  display: flex;
  position: relative;
  color: white;
  font-weight: bold;
  text-decoration: none;
  transition: .2s;
  overflow: hidden; // はみ出た平行四辺形をhiddenする
}

.p-btn--camera2:hover {
  color: midnightblue;
}

.p-btn--camera2::before { // 平行四辺形を乗せているだけ。
  width: 120%; // ベースの四角を覆えればいい大きさ
  height: 100%;
  position: absolute;
  top: 0;
  left: -10%;
  z-index: -1;
  content: '';
  background-color: midnightblue;
  transform: skewX(30deg) scale(1, 1); // 傾き。scaleはノルム
  transition: transform .2s;
}
.p-btn--camera2:hover::before {
  transform: skewX(30deg) scale(0, 1);
}

.p-btn--camera3 {
  width: 150px;
  height: 50px;
  display: flex;
  position: relative;
  color: midnightblue;
  font-weight: bold;
  text-decoration: none;
  transition: .2s;
  overflow: hidden; // はみ出た平行四辺形をhiddenする
}

.p-btn--camera3:hover {
  color: white;
}

.p-btn--camera3::before { // 平行四辺形を乗せているだけ。
  width: 120%; // ベースの四角を覆えればいい大きさ
  height: 100%;
  position: absolute;
  top: 0;
  left: -20%;
  z-index: -1;
  content: '';
  background-color: midnightblue;
  transform-origin: left;
  transform: skewX(-30deg) scale(0, 1); // 傾き。scaleはノルム
  transition: transform .2s;
}
.p-btn--camera3:hover::before {
  transform: skewX(-120deg) scale(0.7, 1);
}

.p-btn--camera3::after { // 平行四辺形を乗せているだけ。
  width: 120%; // ベースの四角を覆えればいい大きさ
  height: 100%;
  position: absolute;
  top: 0;
  right: -20%;
  z-index: -1;
  content: '';
  background-color: midnightblue;
  transform-origin: right;
  transform: skewX(-30deg) scale(0, 1); // 傾き。scaleはノルム
  transition: transform .2s;
}
.p-btn--camera3:hover::after {
  transform: skewX(-120deg) scale(0.7, 1);
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
    // top: -95px;
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
}

.star__1 {
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

.star__2 {
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

.p-btn--bgimage {
  width: 200px;
  height: 170px;
  display: block;
  position: relative;
  background-image: url('../assets/flower.jpg');
  background-size: cover;
  transition-duration: .3s;
  transition-timing-function:ease-out;
  &:hover {
    opacity: 0.7;
  }
}

.p-btn--bgimage:before {
  width: 100px;
  height: 30px;
  display: flex;
  align-items: center;
  justify-content: center;
  position: absolute;
  content: 'test';
  top: 20px;
  right: -10px;
  background-color: rgba(0,0,0,0.3);
  color: white;
}

.p-btn--tagImage {
  width: 200px;
  height: 170px;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  text-decoration: none;
  background-color: #87cefa;
  color: white;
  transition-duration: .3s;
  transition-timing-function:ease-out;
  &:hover {
    opacity: 0.8;
  }
  &::before {
    width: 100px;
    height: 80px;
    display: block;
    position: absolute;
    content: '';
    bottom: -10px;
    right: -10px;
    background-image: url('../assets/flower.jpg');
    background-size: cover;
  }
}

.p-btn__biscuit {
  width: 150px;
  height: 150px;
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 10px;
  margin-bottom: 10px;
  border-radius: 50%;
  background-color: #60452E;
  box-shadow: 0px 0px 0px 8px #60452E;
  border: 1px dashed #443121;
  text-decoration: none;
  text-shadow:#7B583B 0 0 2px;
  color: #443121;
  font-weight: bold;
  font-size: 1.2em;
  &::before, &::after {
    transition-duration: .5s;
    transition-timing-function: ease;
  }
  &::before {
    width: 150px;
    height: 150px;
    position: absolute;
    left: -1px;
    top: 0;
    content: '';
    border-radius: 50%;
    background-color: #60452E;
    box-shadow: 0px 0px 0px 8px #60452E;
    border: 1px dashed #60452E;
    z-index: -2;
  }
  &::after {
    width: 150px;
    height: 150px;
    position: absolute;
    left: 0;
    top: 0;
    content: '';
    border-radius: 50%;
    background-color: white;
    border: 1px solid #60452E;
    z-index: -1;
  }
  &:hover {
    @at-root #{&}::before, #{&}::after{
      left: -40px;
    }
  }
  &:active {
    @at-root #{&}::after{
      background-color: transparentize(white, 0.5);
    }
  }
}

.p-btn__cookie {
  width: 150px;
  height: 150px;
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 10px;
  margin-bottom: 10px;
  border-radius: 50%;
  background-color: #BB9471;
  box-shadow: 0px 0px 0px 8px #BB9471;
  border: 5px dotted #A37A56;
  text-decoration: none;
  color: white;
}

.p-btn__bite {
  width: 150px;
  height: 150px;
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 10px;
  margin-bottom: 10px;
  border-radius: 50%;
  background-color: #BB9471;
  border: 1px solid white;
  text-decoration: none;
  color: white;
  box-sizing: border-box;
  overflow: hidden;
  &::before {
    width: 130px;
    height: 130px;
    position: absolute;
    top: 4px;
    left: 4px;
    content: '';
    border-radius: 50%;
    background-color: transparent;
    border: 5px dotted #A37A56;
  }
  &::after {
    width: 100px;
    height: 100px;
    position: absolute;
    top: -50px;
    right: 0;
    content: '';
    border-radius: 50%;
    background-color: white;
  }
}

</style>
