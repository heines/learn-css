<template lang="pug">
  div
    a.snsShare(@click="shareLine")
      img.lineSize(src='../assets/share-d.png')
</template>


<script>

  export default {
    name: 'lineShare',
    data () {
      return {
      }
    },
    methods: {
      shareLine: function() {
        window.open('https://social-plugins.line.me/lineit/share?url=https://heines.github.io/learn-css/', '_blank');
      }
    }
  }
</script>

<style lang="scss" scoped>
  .snsShare {
    cursor: pointer;
  }
  .lineSize {
    width: 100px;
  }
</style>
