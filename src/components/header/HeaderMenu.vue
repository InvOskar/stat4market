<template>
    <div class="menu">
        <div class="menu_item">
            <p class="item_text">Аналитика</p><div class="item_arrow"><img src="@/assets/img/icons/arrow.svg" ></div>
        </div>
        <div class="menu_item">
            <p class="item_text">Обучение</p>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.menu, .menu_item{
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.menu {
    font-weight: 400;
    font-size: 24px;
    line-height: 35px;

    color: #331A2F;
}
.menu_item{

    &:hover{
        cursor: pointer;
    }
    &:last-child{
        padding-left: 20px;
    }
}
.item_arrow{
    margin-left: 12px;
}
@media (max-width: 1280px) {
    .menu {
        width: 238.54px;
        font-size: 18px;
    }
}
@media (max-width: 768px) {
    .menu {
        display: none;
    }
}
</style>