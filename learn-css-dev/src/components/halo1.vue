<template lang="pug">
  div.baseBox
    h2.title halo
    div.dateBox
      p.date 2018 Oct 28th
    div.descBox
      p.description
        | やりたいことをやった。
        br
        | halo : 暈
    div.contents
      div.halo
        div.filter
          div.sun
    div.elementsDesc
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
@import "../css/halo1.scss";
@import "../css/_layout.scss"
</style>
