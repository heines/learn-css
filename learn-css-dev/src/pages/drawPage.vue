<template lang="pug">
  div
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
</style>
