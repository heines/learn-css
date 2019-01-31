<template lang="pug">
  div
    //- .c-flexbox
    //-   .c-scroll-arrow
    //-     .c-scroll-arrow__box1
    //-     .c-scroll-arrow__box2
    //-     .c-scroll-arrow__box3
    //-     .c-scroll-arrow__up
    //-       .c-scroll-arrow__box1
    //-       .c-scroll-arrow__box1
    //-       .c-scroll-arrow__box1
    //-     .c-scroll-arrow__down
    //-       .c-scroll-arrow__box2
    //-       .c-scroll-arrow__box2
    //-       .c-scroll-arrow__box2
    //-     .c-scroll-arrow__box3
    .p-slide-show
      .p-slide-show__image1
      .p-slide-show__image2
      .p-slide-show__image3
    .c-flexbox
      .p-square-box.p-square-box--bg
        .p-square-box__content-wrap
          .p-square-box__content
            img(src='../assets/pakutaso001.jpg')
      .p-square-box.p-square-box--frame
        .p-square-box__content-wrap
          .p-square-box__content
            p 必ず正方形になる
    .c-flexbox
      .p-open-box
        .p-open-box__main
          p.p-open-box__text
            |hover
        .p-open-box__content
          p.p-open-box__text
            |text
    .c-flexbox
      .p-rolling
        .p-rolling__boll
      .p-box-paper-tag
        |付箋
    .c-flexbox
      p.p-box-shadow-solid(text="文字列に立体的な影がつく（1行のみ）")
        |文字列に立体的な影がつく（1行のみ）
    .c-flexbox
      .p-clapperboard
        .p-clapperboard__clapper
        .p-clapperboard__board
          .p-clapperboard__prodtitle
            |眠い
          .p-clapperboard__date
            |Jan.29th.2019
      .p-scissors
        .p-scissors
          .p-scissors__blade-1
          .p-scissors__blade-2
    .c-flexbox
      .p-checkered
      .p-stripe
      .p-dial
        .p-dial__center
        .p-dial__12
          |12
        .p-dial__1
          |1
        .p-dial__2
          |2
        .p-dial__3
          |3
        .p-dial__4
          |4
        .p-dial__5
          |5
        .p-dial__6
          |6
        .p-dial__7
          |7
        .p-dial__8
          |8
        .p-dial__9
          |9
        .p-dial__10
          |10
        .p-dial__11
          |11
    .c-flexbox
      .p-come-back
        |おすすめメニュー
</template>

<script>
  import star from '../components/star';
  import graph from '../components/graph';
  export default {
    name: 'drawPage',
    data () {
      return {
      };
    },
    components: {
      star,
      graph
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
  @import '../css/_main.scss';
  h1, h2 {
    font-weight: normal;
  }
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
