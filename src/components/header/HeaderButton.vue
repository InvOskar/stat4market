<template>
    <div class="button">
        <img class="icon" src="@/assets/img/icons/headerBtn.svg" />
        <p class="button_text">Войти</p>
    </div>
</template>

<style lang="scss" scoped>
.button {
    width: 169px;
    height: 45px;

    display: flex;
    justify-content: space-between;
    align-items: center;

    padding: 4px 32px;

    background-color: #CF51CE;

    font-weight: 500;
    font-size: 23px;
    line-height: 35px; 
    color: #fff;

    border-radius: 12px;

    &:hover{
        cursor: pointer;
    }

    &>.icon{
        width: 23px;
        height: 23px;
    }
}

@media (max-width: 1280px) {
    .button {
        width: 152px;
        height: 43.88px;

        font-size: 18px;
        line-height: 35px;

        &>.icon{
            width: 20px;
            height: 20px;
        }
    }
}

@media (max-width: 768px) {
    .button {
        width: 158px;
        height: 44px;

        font-size: 20px;
    }
}

@media (max-width: 360px) {
    .button {
        width: 103.21px;
        height: 36px;
        
        padding: 4px 20px;

        font-size: 14px;
        line-height: 28px;  

        &>.icon{
            width: 13.21px;
            height: 13.21px;
        }
    }
}
</style>