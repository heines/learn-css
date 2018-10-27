<template lang="pug">
  div.baseBox
    h2.title 復習1
    div.dateBox
      p.date 2018 Oct 27th
    div.descBox
      p.description
        | flexboxを使用して、divの内部に等間隔に並べる。
        br
        | 両端の幅は等間隔とした幅の半分の大きさとする。
    div.contents
      div.innerContents
        p.innerText1 box1
      div.innerContents
        p.innerText1 box2
      div.innerContents
        p.innerText1 box3
    div.elementsDesc
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
@import "../css/_layout.scss"
</style>
