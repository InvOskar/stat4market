<template>
    <div class="logo-text">
        <div class="logo">
            <img src="@/assets/img/stat4market.svg" alt="Logo" />
        </div>
        <div class="border">
            <p class="text">Надежный сервис<br> аналитики для поставщиков<br> на маркетплейсы</p>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.logo-text, .logo, .text {
    display: flex;
    align-items: center;
}
.logo-text{
    width: auto;
    height: auto;
}
.border{
    border-left: 2px solid rgba(51, 26, 47, 0.5);
    margin-left: 19px;
}
.text{
    padding-left: 25px;

    height: 80px;
    font-weight: 400;
    font-size: 14px;
    line-height: 18px;

    color: rgba(51, 26, 47, 0.9);
}
</style>