<template>
    <div class="main" v-if="width>768">
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
    <div class="main" v-else-if="width>360">
        <p class="header_text">
            <span>Обучающие курсы</span> для поставщиков на маркетплейсы
        </p>
        <div class="inner-block">
            <div class="left-side">
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
                <img src="@/assets/img/Superman2.png" alt="">
            </div>
        </div>
    </div>
    <div class="main" v-else>
        <div class="inner-block">
            <p class="header_text">
                <span>Обучающие курсы</span> для поставщиков на маркетплейсы
            </p>
            <div class="right-side">
                <img src="@/assets/img/Superman2.png" alt="">
            </div>
        </div>
        <div class="left-side">
            <div class="price">
                <img src="@/assets/img/icons/spent.svg" alt="">
                <p class="price_text">
                    от <span>19 900</span> ₽
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
    </div>
</template>

<script>
export default {
    data() {
        return {
            width: window.innerWidth,
        }
    },
    mounted() {
        window.addEventListener('resize', () => {
            this.width = window.innerWidth;
        });
    }
}
</script>

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

@media (max-width: 1280px) {
    .header_text{
        font-size: 46px;
        line-height: 65px;
    }
    .price{
        padding: 40px 0;
    }
    .text{
        font-size: 20px;
    }
    .right-side {
        &>img{
            width: 458.35px;
        }
    }
}

@media (max-width: 768px) {
    .main{
        flex-direction: column;

        &>.inner-block{
            display: flex;
        }
    }
    .price{
        padding: 18px 0;
    }
    .right-side {
        right: -23px;

        &>img{
            width: 241px;
            height: 410px;
        }
    }
}

@media (max-width: 360px) {
    .header_text{
        padding-top: 44px;
        font-size: 26px;
        line-height: 150%;
    }
    .price{
        padding-top: 24px;
        padding-bottom: 16px;
    }
    .text{
        font-size: 18px;
    }
    .right-side {
        right: -15px;
        &>img{
            width: 140px;
            height: 245px;
        }
    }
}
</style>