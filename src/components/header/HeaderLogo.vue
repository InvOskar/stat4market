<template>
    <div class="logo-text">
        <div class="logo">
            <img src="@/assets/img/stat4market.svg" alt="Logo" />
        </div>
        <div class="border">
        </div>
        <p class="text">Надежный сервис<br> аналитики для поставщиков<br> на маркетплейсы</p>
    </div>
</template>

<style lang="scss" scoped>
.logo-text{
    display: flex;
    justify-content: space-between;
    align-items: center;

    width: 489px;
}
.logo>img{
    width: 100%;
}
.border{
    border: 0.777096px solid rgba(51, 26, 47, 0.5);
    height: 80px;
    
    margin-left: 10px;
}
.text{
    font-weight: 400;
    font-size: 14px;
    line-height: 18px;
    padding-left: 10px;

    color: rgba(51, 26, 47, 0.9);
}

@media (max-width: 1280px) {
    .logo-text{
        width: 380px;
    }
    .border{
        height: 62px;
    }
    .text{
        font-weight: 400;
        font-size: 10px;
        line-height: 14px;
    }
}
@media (max-width: 768px) {
    .logo-text{
        width: 372px;
    }
}
@media (max-width: 360px) {
    .logo-text{
        width: 140px;
    }
    .text, .border{
        display: none;
    }
}

</style>