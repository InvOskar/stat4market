<template>
    <div class="header">
        <header-logo/>
        <header-menu/>
        <header-phone/>
        <header-button/>
    </div>
</template>

<script>
import HeaderButton from './HeaderButton.vue'
import HeaderMenu from './HeaderMenu.vue'
import HeaderLogo from './HeaderLogo.vue'
import HeaderPhone from './HeaderPhone.vue'
export default {
  components: { HeaderButton, HeaderMenu, HeaderLogo, HeaderPhone },

}
</script>

<style lang="scss" scoped>
.header {
    display: flex;
    justify-content: space-between;
    align-items: center;

    padding: 35px 195px;
    margin: auto;
}
@media (max-width: 1280px) {
    .header {
        padding: 35px 40px;
    }
}
@media (max-width: 768px) {
    .header {
        padding: 35px 23px 35px 16px;
    }
}
@media (max-width: 360px) {
    .header {
        padding: 35px 15px;
    }
}
</style>