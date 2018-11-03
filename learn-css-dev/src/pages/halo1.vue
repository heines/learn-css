<template lang="pug">
  div.base-box
    h2.title halo
    div.date-box
      p.date-box_text 2018 Oct 28th
    div.desc-box
      p.desc-box_text
        | やりたいことをやった。
        br
        | halo : 暈
    div.contents
      div.halo
        div.filter
          div.sun
    div.elements-desc
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
@import "../css/Layout/_layout.scss"
</style>
