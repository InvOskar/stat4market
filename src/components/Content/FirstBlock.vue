<template>
    <div class="main">
        <div class="left-side">
            <p class="header_text">
                <span>Обучающие курсы</span> для поставщиков на маркетплейсы
            </p>
            <div class="price">
                <img src="@/assets/img/icons/spent.svg" alt="">
                <p class="price_text">
                    от <span>19 900</span> &#x20bd;
                </p>
            </div>
            <div class="text">
                <p>
                    Обучающие курсы по работе и продвижению на маркетплейсах от практикующих селлеров
                </p>
                <p>
                    Добро пожаловать в Академию. Это место для эффективного обучения, где мы рассказываем, как работают маркетплейсы и никогда не вдаемся в теорию, которая не понадобится на практике.
                </p>
                <p>
                    Нащи уроки помогут понять логику работы площадок и взять управление продажами в свои руки, а не действовать наугад. Становись экспертом в работе с маркетплейсами и увеличивай свою прибыль.
                </p>
            </div>
        </div>
        <div class="right-side">
            <img src="@/assets/img/Superman.png" alt="">
        </div>
    </div>
</template>

<style lang="scss" scoped>
.main {
    display: flex;
    justify-content: space-between;
}
.left-side {
    color: rgba(51, 26, 47, 0.8);
}
.header_text {
    font-weight: 700;
    font-size: 56px;
    line-height: 80px;

    &>span{
        color: #CF51CE;
    }
}
.price{
    display: flex;
    align-items: center;

    padding-top: 22px;

    &>.price_text{
        
        padding-left: 25px;
        font-weight: 600;
        font-size: 20px;
        line-height: 29px;

        &>span{
            font-weight: 700;
            font-size: 38px;
            line-height: 55px;
            color: #CF51CE;
        }
    }
}
.text{
    padding-top: 16px;
    padding-right: 39px;
    
    font-weight: 400;
    font-size: 25px;
    line-height: 160%;

    display: grid;
    grid-gap: 15px;
}
.right-side {
    pointer-events: none;

    position: relative;
}
</style>