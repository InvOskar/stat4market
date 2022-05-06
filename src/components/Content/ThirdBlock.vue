<template>
    <div class="main">
        <div class="header_text">
            Обучение по продажам на маркетплейсах от <p>stat<span class="color">4</span>market<div class="underline"></div></p>
        </div>
        <p class="secondary_text">
            «Увеличение реальной прибыли, конкретика и ключевые инструменты, которые дают результат» — на этом тезисе созданы наши курсы
        </p>
    </div>
    
</template>

<style lang="scss" scoped>
.main {
    margin-top: -7px;
    text-align: center;
}
.header_text{
    font-weight: 700;
    font-size: 48px;
    line-height: 64px;

    width: 679px;
    margin: auto;

    &>span{
        color: #CF51CE;
    }
}
.underline{
    width: 261px;
    height: 7px;

    display: block;
    margin: auto;

    background: linear-gradient(264.91deg, #7C4EAB 0.73%, #DD51D4 95.85%);
    border-radius: 5px;

}
.secondary_text{
    padding-top: 23px;

    font-weight: 400;
    font-size: 25px;
    line-height: 160%;

    color: rgba(51, 26, 47, 0.8);

    max-width: 846px;
    margin: auto;
}

@media (max-width: 1280px) {
    .header_text{
        font-size: 40px;
        line-height: 64px;
        max-width: 641.96px;
    }
    .underline{
        width: 218px;
        height: 6px;
    }
    .secondary_text{
        font-size: 20px;
        line-height: 160%;
        max-width: 683.96px;
    }
}
@media (max-width: 768px) {
    .header_text{
        max-width: 626px;
    }
}
</style>