<template lang="pug">
  div.base-box
    h2.title 予習
    div.date-box
      p.date 2018 Oct 30th (29th)
    div.desc-box
      p.description
        | バルーンを表示する。以下より主要部分だけ抜き出し。
        br
        | 参考:
        a(href='https://qiita.com/kazu69/items/6f911fb41e88505142c7') シンプルなhtmlとcssのみでできるツールチップ
        br
        | z-index:9999とか嫌い。
        br
        | 難しくて分からなかったのでもう一回やる。
    div.contents
      div.box
        span.tooltip.top(aria-label="balloon")
          | text hover show tooltip bottom
    div.elements-desc
      dl
        dt content: attr();
          dd 関数。指定の要素の属性の値を受け取り、スタイルシート内で使用できる。
        dt z-index
          dd 値が大きいほど前面に配置される。
</template>

<script>

export default {
  name: 'baloon',
  data () {
    return {
    }
  }
}
</script>

<style lang="scss" scoped>
@import "../css/balloon.scss";
@import "../css/_layout.scss"
</style>
