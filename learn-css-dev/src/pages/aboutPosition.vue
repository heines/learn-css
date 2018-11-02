<template lang="pug">
  div.base-box
    h2.title 絶対位置・相対位置
    div.date-box
      p.date-box_text 2018 Oct 30th
    div.desc-box
      p.desc-box_text
        | バルーンとかやる前に、そもそもabsoluteを理解していない疑惑。
        br
        | 丸いのがrelative、半透明の四角がabsolute
    div.contents
      div.box1
        div.box2
          div.box3
            p test text
    div.elements-desc
      dl
        dt position:static
          dd デフォルト値。何も指定してないときはこれ。
        dt position:relative
          dd 本来 （static）の位置からのずれ。
        dt position:absolute
          dd
            |親要素がstaticの場合はウィンドウ左上端からのずれ。
            br
            |親要素がrelative/fixedの場合は、親要素左上端からのずれ。
</template>

<script>

export default {
  name: 'aboutPosition',
  data () {
    return {
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../css/aboutPosition.scss";
@import "../css/_layout.scss"
</style>
