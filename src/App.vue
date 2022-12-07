<template>
	<div id="app">
		<HeaderPage />
		<MainPage />
		<FooterPage />
	</div>
</template>

<script>
import HeaderPage from "./components/HeaderPage.vue";
import MainPage from "./components/MainPage.vue";
import FooterPage from "./components/FooterPage.vue";

export default {
	name: "App",
	components: {
		HeaderPage,
		MainPage,
		FooterPage,
	},
};
</script>

<style lang="scss">
@import "./css/global.scss";
@import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@200;300;400;500;600;700;800&display=swap');
</style>
