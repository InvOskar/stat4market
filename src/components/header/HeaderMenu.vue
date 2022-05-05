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
    gap: 50px;
    font-weight: 400;
    font-size: 24px;
    line-height: 35px;

    color: #331A2F;
}
.menu_item{
    gap: 11.45px;

    &:hover{
        cursor: pointer;
    }
}

@media (max-width: 1280px) {
    .menu {
        gap: 40.45px;
        font-size: 18px;
    }
    .menu_item{
        gap: 12px;
    }
}
@media (max-width: 768px) {
    .menu {
        display: none;
    }
}
</style>