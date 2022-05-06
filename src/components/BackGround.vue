<template>
    <div class="bg-image">
        <img src="~@/assets/img/BG-Ellipse.png" alt="">
        <img src="~@/assets/img/BG-Ellipse-1.png" alt="">
        <img src="~@/assets/img/BG-Ellipse-2.png" alt="">
    </div>
</template>

<style lang="scss" scoped>
.bg-image {
  position: absolute;

  &>img{
    position: absolute;
    pointer-events: none;

    &:nth-child(1) {
      top: 0;
      left: 0;
    }
    &:nth-child(2) {
      top: 385px;
      left: calc(100vw - 58px);
    }
    &:nth-child(3) {
      top: 0;
      left: 0;
      display: none;
    }
  }
}

@media (max-width: 1280px){
    .bg-image {
        &>img:nth-child(1), &>img:nth-child(2) {
            display: none;
        }
        &>img:nth-child(3) {
            display: block;
        }
    }
}

@media (max-width: 768px){
    .bg-image {
        &>img:nth-child(3) {
            display: none;
        }
    }
}
</style>