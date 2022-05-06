<template>
    <div>
        <div class="icon">
            <img :src="require(`@/assets/img/icons/${card.icon}.svg`)" alt="">
        </div>
        <div class="text">
            <p class="title">{{card.title}}</p>
            <p class="description">{{card.text}}</p>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        card: {
            type: Object,
            required: true
        }
    }
}
</script>

<style lang="scss" scoped>
.icon {
    width: 70px;
    height: 70px;

    background: #CF51CE;
    box-shadow: 0px 4px 25px rgba(234, 93, 187, 0.25);
    border-radius: 15px;

    display: flex;
    justify-content: center;
    align-items: center;
}
.text {
    padding-top: 30px;

    &>.title {
        font-weight: 600;
        font-size: 24px;
        line-height: 150%;

        padding-right: 50px;
    }
    &>.description {
        padding-top: 15px;
        font-weight: 400;
        font-size: 18px;
        line-height: 160%;
        color: rgba(51, 26, 47, 0.8);
    }
}

@media (max-width: 1280px) {
    .icon {
        width: 60px;
        height: 60px;
        &>img{
            width: 65%;
        }
    }
    .text{
        padding-top: 20px;

        &>.title {
            font-size: 20px;
            line-height: 150%;
            padding-right: 0;
        }
        &>.description {
            padding-top: 10px;
            font-size: 16px;
            line-height: 160%;
        }
    }
}
@media (max-width: 360px) {
    .icon{
        margin: auto;
    }
    .text{
        text-align: center;
        &>.title {
            font-size: 18px;
            line-height: 150%;
        }
    }

}
</style>