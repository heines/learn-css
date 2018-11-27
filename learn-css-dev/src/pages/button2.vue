<template lang="pug">
  .base-box
    .contents
      .contents-section
        hamburger
    .elements-desc
      dl
        dt transition
          dd
            li 変化する対象
            li 変化する時間
            li 変化する速度変化
            li 変化開始までの時間
            | を指定できる。
</template>

<script>
  import hamburger from '../components/hamburger';
  export default {
    name: 'button1',
    components: {
      hamburger
    }
  }
</script>

<style lang="scss" scoped>
  @import "../css/Layout/_layout.scss";

  .contents {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 500px;
    height: 150px;
  }

  .desc-box_text {
    text-align: left;
  }

  .contents-section {
    margin: 10px 0;
  }

</style>
