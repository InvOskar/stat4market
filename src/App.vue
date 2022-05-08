<template>
	<div class="app">
    	<main-page/>
	</div>
</template>

<script>
import MainPage from './components/MainPage.vue'

export default {
  components: { MainPage },
  
}
</script>

<style lang="scss">
@import "http://fonts.fontstorage.com/import/lato.css";
*{
	margin: 0;
	padding: 0;
	box-sizing: border-box;
	font-family: 'Lato';
}
</style>
