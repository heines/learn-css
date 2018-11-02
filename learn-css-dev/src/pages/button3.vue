<template lang="pug">
  .base-box
    h2.title 予習
    .date-box
      p.date-box_text 2018 Nov 3rd (2nd)
    .desc-box
      p.desc-box_text ボタンを作るその3
        br
        |波紋を作ろうとしたけどできなかった。
        br
        |グラデーションはtransitionもanimationもできない。
        br
        |今日はリファクタリングとカーソルの勉強に終始。
    .contents
      .contents-section
        ripple
</template>

<script>
import ripple from '../components/ripple';
export default {
  name: 'button3',
  components: {
    ripple
  }
}
</script>

<style lang="scss" scoped>
@import "../css/_layout.scss"
</style>
