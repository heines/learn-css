<template lang="pug">
  div.errorBox
    h2 error test
    p fixed は画面に対して固定
      br
      |消す方法はまたあとで考える。
</template>

<script>
export default {
  name: 'errorPage',
  data () {
    return {
    };
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
h1, h2 {
  font-weight: normal;
}
.errorBox {
  width: 800px;
  height: 500px;
  position: fixed;
  top: calc(50% - 250px);
  left: calc(50% - 400px);
  z-index: 1;
  background-color: rgba(135, 206, 250, 0.8);
}
</style>
