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
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
	font-family: Lato;
}

@font-face {
	font-family: "Lato";
	font-style: normal;
	font-weight: 300;
	src: url("~@/assets/fonts/Lato/Lato-Light.ttf");
}
@font-face {
	font-family: "Lato";
	font-style: normal;
	font-weight: 400;
	src: url("~@/assets/fonts/Lato/Lato-Regular.ttf");
	src: url("~@/assets/fonts/Lato/Lato-Regular.ttf") format("truetype");
}
@font-face {
	font-family: "Lato";
	font-style: normal;
	font-weight: 800;
	src: url("~@/assets/fonts/Lato/Lato-Bold.ttf");
	src: url("~@/assets/fonts/Lato/Lato-Bold.ttf") format("truetype");
}
@font-face {
	font-family: "Lato";
	font-style: normal;
	font-weight: 900;
	src: url("~@/assets/fonts/Lato/Lato-Black.ttf");
	src: url("~@/assets/fonts/Lato/Lato-Black.ttf") format("truetype");
}
</style>
