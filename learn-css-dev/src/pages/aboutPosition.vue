<template lang="pug">
  .base-box
    h2.title 絶対位置・相対位置
    .date-box
      p.date-box_text 2018 Oct 30th
    .desc-box
      p.desc-box_text
        | バルーンとかやる前に、そもそもabsoluteを理解していない疑惑。
        br
        | 丸いのがrelative、半透明の四角がabsolute
    .contents
      .box1
        .box2
          .box3
            p test text
    .elements-desc
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
@import "../css/Layout/_layout.scss";

.contents {
  width: 500px;
  height: 300px;
  margin: 20px;
  border: 1px solid #CCCCCC;
}

.box1 {
  width: 200px;
  height: 200px;
  background-color: #87cefa;
}

.box2 {
  width: 100px;
  height: 100px;
  position: relative;
  left: 20px;
  top: 30px;
  background-color: white;
  box-sizing: border-box;
  border-radius: 50px;
}

.box3 {
  width: 100px;
  height: 100px;
  position: absolute;
  content: "test";
  left: 25px;
  top: 25px;
  color: black;
  background-color: rgba(144, 144, 144, 0.5);
}

.inner-absolute {
  display: block;
}

</style>
