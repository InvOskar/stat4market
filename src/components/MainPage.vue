<template>
  <div class="main-page">
    <back-ground/>
    <the-header/>
    <div class="content">
      <p class="upper-text">Главная - Обучение</p>
      <first-block/>
      <second-block/>
      <third-block/>
      <forth-block/>
    </div>
  </div>
</template>

<script>
import BackGround from './BackGround.vue'
import TheHeader from './header/TheHeader.vue'
import FirstBlock from './Content/FirstBlock.vue'
import SecondBlock from './Content/SecondBlock.vue'
import ThirdBlock from './Content/ThirdBlock.vue'
import ForthBlock from './Content/ForthBlock.vue'

export default {
  components: { TheHeader, BackGround, FirstBlock, SecondBlock, ThirdBlock, ForthBlock },
  
}
</script>

<style lang="scss" scoped>
.content {
  margin: auto;
  margin-top: 31px;

  padding: 0 10%;
}
.upper-text {
  font-weight: 400;
  font-size: 16px;
  line-height: 19px;

  color: rgba(51, 26, 47, 0.5);
}
@media (max-width: 1280px) {
  .content {
    padding: 0 5%;
  }
}
@media (max-width: 768px) {
  .content {
    padding: 0 23px;
  }
}
@media (max-width: 360px) {
  .content {
    padding: 0 15px;
  }
}
</style>