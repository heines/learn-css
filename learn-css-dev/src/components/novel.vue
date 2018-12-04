<template lang="pug">
  .p-novel
    .p-novel__paper
      h2.p-novel__title 彼は誰
      h3.p-novel__name 清水灰猫
      .p-novel__story
        p.p-novel__story--first
          |氷点下二度。暖房も点けずに眠っていた私は、その朝、あまりの寒さに目を覚ました。部屋の中だというのに吐く息が白い。自力で表面体温を上げることを早々に諦め、布団を出てエアコンの電源を入れる。
        p.p-novel__story--text
          |カーテンの隙間から、弱い光が部屋に入り込む。日はまだ昇っていない。私は、何の気なしにその隙間から外を臨む。
        p.p-novel__story--text
          |暗い西の空、天頂に近くなるに従って闇色から薄く光を帯びた。一瞬緑色を映し、黄色、橙と色を変え、東の空の縁を赤く染める。その空を、ささやかに星が一つ飾っていた。
        p.p-novel__story--text
          |明けの明星。あれが恒星でないと教えてくれた人は、一体誰だったか。
        p.p-novel__story--text
          |人の気配を感じ、私はそっとカーテンを引いた。
        p.p-novel__story--text__under
          |ドロップキャップと字下げの相性が悪い。あと、safariだとfirst-letterにおけるfloat: leftの動作がおかしい。
</template>

<script>
export default {
  name: 'novel',
  data () {
    return {
    }
  }
}
</script>

<style lang="scss" scoped>
  @import '../css/_variables.scss';
  .p-novel {
    font-family:serif;
    margin: 10px;
    color: hsl(0%, 0%, 32%);
  }
  .p-novel__paper {
    padding: 10px;
    background-color: hsl(50%, 100%, 97%);
  }
  .p-novel__title {
    margin: 0;
    text-align: left;
    padding-left: 1em;
    background-color: rgba(0, 0, 0, 0.05);
  }
  .p-novel__name {
    font-size: 0.9em;
    text-align: right;
    border-bottom: 1px solid rgba(0, 0, 0, 0.05);
  }

  .p-novel__story {
    text-align: left;
    margin: 0;
    &--text {
      margin: 0;
      &__under {
        margin: 0;
        text-indent: 1em;
      }
    }
    &--first {
      margin: 0;
      &::first-letter {
        text-indent: 1em;
        margin-right: 0.1em;
        color: $midnight;
        font-size: 3em;
        line-height: 1;
      }
    }
  }
</style>
