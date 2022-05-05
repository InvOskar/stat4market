<template>
  <div class="app">
    <the-header/>
  </div>
</template>

<script>
import TheHeader from './components/header/TheHeader.vue'

export default {
  components: { TheHeader },
  
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

@font-face {
  font-family: 'Lato';
  src: url();
}
</style>
