<template lang="pug">
  .p-manuscript
    .p-manuscript__paper
      .p-manuscript__title ハロー
      .p-manuscript__name 清水 灰猫
      .p-manuscript__textarea
        .p-manuscript__text__outer
          .p-manuscript__text
            |「どうして、ヒトだけが特別だなんて思ったの？」
            br
            |　彼女は、興味がない、という体で頬杖をつく。運悪く箱舟に乗せられた俺は、ただの実験動物に過ぎない。
            br
            |「……可哀想にね」
            br
            |　彼女にとって、猫も犬も人間も、総じて生き物、という括りでしかない。二百年も生きていれば、そうなって然るべきなのか、そうではないのか。人並みの寿命しか持ち合わせていないだろう自分には、想像もつかなかった。
        .p-manuscript__fish
        .p-manuscript__text__outer
          .p-manuscript__text
            |　ちなみに、原稿用紙の真ん中にある模様は、「魚尾」と呼ばれるもので、半分にして折ることを前提とした印である。
            br
            |　結局 grid レイアウトを使用した。
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
  @import '../css/Object/Project/_manuscript.scss';
</style>
