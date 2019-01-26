<template lang="pug">
  div
    .p-slide-show
      .p-slide-show__image1
      .p-slide-show__image2
      .p-slide-show__image3
    .c-square-box
      .c-square-box__content-wrap
        .c-square-box__content
          img(src='../assets/pakutaso001.jpg')
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
  @import '../css/Object/Project/_slide-show.scss';
  @import '../css/Object/Component/_square_box.scss';
  h1, h2 {
    font-weight: normal;
  }
</style>
