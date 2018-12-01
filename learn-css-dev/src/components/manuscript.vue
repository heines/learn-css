<template lang="pug">
  .p-manuscript
    .p-manuscript__paper
      .p-manuscript__title ハロー
      .p-manuscript__name 清水 灰猫
      .p-manuscript__text__outer
        .p-manuscript__text
          |「どうして、ヒトだけが特別だなんて思ったの？どうでもいいけど」
          br
          |　彼女は、興味がない、という体で頬杖をつく。運悪く箱舟に乗せられた俺は、ただの実験動物に過ぎない。
          br
          |「……可哀想にね」
          br
          |　彼女にとって、猫も犬も人間も、総じて生き物、という括りでしかない。二百年も生きていれば、そうなって然るべきなのか、そうではないのか。人並みの寿命しか持ち合わせていないだろう自分には、想像もつかなかった。
        .p-manuscript__fish
        .p-manuscript__text
          |　ちなみに、原稿用紙の真ん中にある模様は、「魚尾」と呼ばれるもので、半分にして折ることを前提とした印である。
</template>

<script>
export default {
  name: 'manuscript',
  data () {
    return {
    }
  }
}
</script>

<style lang="scss" scoped>
  .p-manuscript {
    width: 100%;
    padding: 10px;
    box-sizing: border-box;
    &__paper {
      width: 100%;
      height: 500px;
      padding: 50px;
      box-sizing: border-box;
      overflow:scroll;
      background-color: hsl(50%, 100%, 97%);
      font-family:serif;
      color: hsl(0%, 0%, 32%);
      writing-mode: vertical-rl;
    }
    &__text__outer {
    }
    &__title {
      padding-top: 3em;
      padding-left: 1em;
      text-align: left;
    }
    &__name {
      padding-left: 1em;
      padding-bottom: 1em;
      text-align: right;
    }
    &__text {
      width: calc(50% - 18px);
      text-align: left;
    }
    &__fish {
      width: 20px;
      position: relative;
      margin-right: .5em;
      margin-left: .5em;
      &::before {
        position: absolute;
        top: 20%;
        right: 0;
        content: '';
        border-top: 3px solid hsl(40%, 100%, 30%);
        border-right: 10px solid hsl(40%, 100%, 30%);
        border-left: 10px solid hsl(40%, 100%, 30%);
        border-bottom: 3px solid hsl(50%, 100%, 97%);
        box-sizing: border-box;
      }
      &::after {
        width: 20px;
        height: 3px;
        position: absolute;
        bottom: 20%;
        right: 0;
        content: '';
        background-color: hsl(40%, 100%, 30%);
      }
    }
  }
</style>
