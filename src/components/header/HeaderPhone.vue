<template>
    <div class="phone">
        <img class="phone-icon" src="@/assets/img/icons/phone.svg" alt="Phone" />
        <p class="phone-number">&nbsp;8 (499) 450-31-41 </p>
    </div>
</template>

<style lang="scss" scoped>
.phone{
    width: 232px;
    height: 36px;

    display: flex;
    justify-content: space-between;
    align-items: center;
    
    &>.phone-icon{
        width: 18.76px;
        height: 18.76px;
        fill: #331A2F;
    }
    &>.phone-number{
        font-weight: 400;
        font-size: 24px;
        line-height: 35px;
        color: #331A2F;

        width: 203px;

        border: 1px solid black;
    }
}

@media (max-width: 1280px) {
    .phone {
        width: 174px;
        
        &>.phone-icon{
            width: 15.63px;
            height: 15.58px;
        }
        &>.phone-number{
            font-size: 18px;

            width: 152px;

            border: 1px solid black;
        }
    }
}

@media (max-width: 768px) {
    .phone {
        display: none;
    }
}
</style>