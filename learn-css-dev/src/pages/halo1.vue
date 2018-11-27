<template lang="pug">
  .base-box
    h2.title halo
    .date-box
      p.date-box_text 2018 Oct 28th
    .desc-box
      p.desc-box_text
        | やりたいことをやった。
        br
        | halo : 暈
    .contents
      .halo
        .filter
          .sun
    .elements-desc
      dl
        dt background: radial-gradient()
          dd 円形グラデーションを指定（中心からの放射方向）
        dt background-color: rgba()
          dd RGBAカラーモデルで色を指定（アルファ値が指定できる）
</template>

<script>
  export default {
    name: 'halo1',
    data () {
      return {
      }
    }
  }
</script>

<style lang="scss" scoped>
  @import "../css/Layout/_layout.scss";
  @import '../css/_variables.scss';

  .contents {
    margin: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 500px;
    height: 500px;
    background-color: $sky;
  }

  .halo {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 400px;
    height: 400px;
    // background: radial-gradient(circle farthest-side, white 30px, $sky 50px, $sky 170px, #fad0c8, #fafac8, #c8e9fa, $sky);
    background: radial-gradient(circle farthest-side, $sky 180px, #fad0c8, #fafac8, #c8e9fa, $sky);
  }

  .filter {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 400px;
    height: 400px;
    background-color: rgba(230, 238, 255, 0.7);
  }

  .sun {
    width: 100px;
    height: 100px;
    background: radial-gradient(circle farthest-side, white, white, $sky);
  }

</style>
