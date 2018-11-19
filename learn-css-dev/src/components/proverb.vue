<template lang="pug">
  .p-prov
    .p-prov__paper
      h2.p-prov__text One today is worth two tomorrow.
</template>

<script>
export default {
  name: 'proverb',
  data () {
    return {
    }
  }
}
</script>

<style lang="scss" scoped>
.p-prov {
  font-family:serif;
  margin: 10px;
  color: hsl(0%, 0%, 32%);
}
.p-prov__paper {
  padding: 10px;
  background-color: hsl(50%, 100%, 97%);
}

.p-prov__text {
  font-size: 1.2em;
  animation-name: slideIn, fadeIn;
  animation-duration: 1s;
  animation-timing-function: ease-in;
  animation-fill-mode: both;
  animation-iteration-count: 1;
}

@keyframes slideIn {
  0% {
    transform: translateX(2em);
  }
  100% {
    transform: translateX(0);
  }
}

@keyframes fadeIn {
  0% {
    opacity: 0;
  }
  50% {
    opacity: 0.6;
  }
  100% {
    opacity: 1;
  }
}

</style>
