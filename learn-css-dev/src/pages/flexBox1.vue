<template lang="pug">
  .base-box
    h2.title 復習1
    .date-box
      p.date-box_text 2018 Oct 27th
    .desc-box
      p.desc-box_text
        | flexboxを使用して、divの内部に等間隔に並べる。
        br
        | 両端の幅は等間隔とした幅の半分の大きさとする。
    .contents
      .innerContents
        p.innerText1 box1
      .innerContents
        p.innerText1 box2
      .innerContents
        p.innerText1 box3
    .elements-desc
      dl
        dt justify-content:space-around;
          dd 水平方向の並びを等間隔にする
        dt align-items: center;
          dd 垂直方向の並びを中央揃えにする
        dt display: block;
          dd ブロック要素として扱う。（文字に使用）
</template>

<script>

export default {
  name: 'flexbox1',
  data () {
    return {
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../css/flexbox1.scss";
@import "../css/Layout/_layout.scss"
</style>
