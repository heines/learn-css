<template lang="pug">
  div.base-box
    h2.title 復習
    div.date-box
      p.date 2018 Nov 1st (Oct 31st)
    div.desc-box
      p.description aタグだけでボタンを作る
    div.contents
      div.contents-section
        a.button_a(href="#")
        p ボタンらしいって難しい
      div.contents-section
        div.tab_set
          a.tab_a(href="#") 1
          a.tab_b(href="#") 2
          a.tab_a(href="#") 3
        p タブっぽいな
    div.elements-desc
      ul
        li 目新しい要素はなし。
        li 親要素display:flexにすると潰れる。（理由は不明）
</template>

<script>

export default {
  name: 'button1',
  data () {
    return {
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../css/button1.scss";
@import "../css/_layout.scss"
</style>
