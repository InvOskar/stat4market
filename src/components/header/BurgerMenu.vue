<template>
    <div class="burger-menu">
        <div class="line"></div>
        <div class="line"></div>
        <div class="line"></div>
    </div>
</template>

<style lang="scss" scoped>
.burger-menu {
    margin-left: 10px;

    width: 42px;
    height: 28px;

    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: flex-end;

    display: none;
}
.line{
    width: 42px;
    height: 4px;
    background: #CF51CE;
    border-radius: 4px;

    &:last-child{
        width: 32px;
    }
}

@media (max-width: 768px) {
    .burger-menu {
        display: flex;
    }
}
</style>