<template>
    <div class="main">
        <p class="header_text">Небольшая предыстория о том, почему нам можно доверять</p>
        <div class="container">
            <div class="image1">
                <img src="@/assets/img/picture-2.1.png" alt="">
            </div>
            <div class="content">
                <p class="text">
                    Свой путь в бизнесе мы начали в 2016 г. У нас были свои островные магазины в крупных ТЦ Москвы («Европейский», «Метрополис», «Мега» и др.), а также свой интернет-магазин. Мы накопили большой опыт в продвижении своих товаров за счет многочисленных запусков разных рекламных каналов и работы с блогерами.
                </p>
            </div>
        </div>
        <div class="container">
            <div class="content">
                <p class="text">
                    Летом 2019 года мы вышли на маркетплейсы и после работы с ними в течение 2 месяцев приняли решение развивать только это направление. И не прогадали. Весь накопленный опыт мы направили на улучшение и продвижение наших брендов.
                </p>
                <p class="text">
                    Пришло время поделится знаниями и лайфхаками, которые будут собраны и доступны в нашей Академии stat4market.
                </p>
            </div>
            <div class="image2">
                <img src="@/assets/img/picture-2.2.png" alt="">
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.main {
    padding: 140px 215px;
    color: rgba(51, 26, 47, 0.8);
}
.header_text {
    font-weight: 700;
    font-size: 48px;
    line-height: 64px;

    width: 844px;
    margin: auto;
    padding-bottom: 85px;

    text-align: center;
}
.container {
    display: flex;
    align-items: center;

    font-weight: 400;
    font-size: 25px;
    line-height: 160%;

    &>div:nth-child(2){
        padding-left: 80px;
    }
}
.content {
    &>p:nth-child(2) {
        margin-top: 15px;
    }
}

@media (max-width: 1280px) {
    .main{
        padding: 77px 103px;
    }
    .header_text{
        font-size: 40px;
        width: auto;
    }
    .container{
        font-size: 20px;
    }
    .image1>img{
        width: 352px;
    }
    .image2>img{
        width: 358px;
    }
}
@media (max-width: 768px){
    .main{
        padding: 65px 5%;
    }
    .header_text{
        padding-bottom: 80px;
    }
    .container{
        &>div:nth-child(2){
            padding-left: 40px;
        }
    }
    .image1>img{
        width: 270px;
    }
    .image2>img{
        width: 270px;
    }
}
@media (max-width: 360px){
    .main{
        padding: 85px 0;
    }
    .header_text{
        padding-bottom: 50px;
    }
    .container{
        flex-direction: column;
        justify-content: center;
        
        &:last-child{
            margin-top: 40px;
            flex-direction: column-reverse;
        }
        &>div:nth-child(2){
            padding: 0;
        }
    }
}
</style>