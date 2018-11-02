<template lang="pug">
  .base-box
    h2.title 復習2
    .date-box
      p.date-box_text 2018 Nov 2nd (1st)
    .desc-box
      p.desc-box_text ボタンを作るその2。
        br
        |ハンバーガーのボタンだけ作る。
        br
        |今回はCSSだけじゃないのでコンポーネント化した。
        br
        |これでクラスのオンオフつければメニューに使える気がする。
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
@import "../css/button2.scss";
@import "../css/_layout.scss"
</style>
