<template lang="pug">
  .errorBox
    h2 error test
    p
      |fixed は画面に対して固定
      br
      |消せるけど方法（ソース）がいまいち。
    .btn(@click="closeErrorPage") close
</template>

<script>
  export default {
    name: 'errorPage',
    data () {
      return {
      };
    },
    methods :{
      closeErrorPage : function(){
        this.$parent.isError = '';
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
  @import '../css/_variables.scss';
  h1, h2 {
    font-weight: normal;
  }
  .errorBox {
    width: 800px;
    height: 500px;
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    position: fixed;
    top: calc(50% - 250px);
    left: calc(50% - 400px);
    z-index: 1;
    background-color: rgba(135, 206, 250, 1.0);
  }

  .btn {
    width: 200px;
    height: 50px;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: white;
    color: $midnight;
    &:hover {
      opacity: 0.7;
    }
  }
</style>
