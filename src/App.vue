<template>
	<div id="app">
		<div id="fixex-menu-container">
			<div id="fixed-menu">
				<div id="linkside1"><i class="fa-solid fa-triangle-exclamation"></i></div>
				<div id="linkside2"><i class="fa-solid fa-life-ring"></i></div>
				<div id="linkside3"><i class="fa-solid fa-sheet-plastic"></i></div>
				<div id="linkside4"><i class="fa-solid fa-cart-shopping"></i></div>
			</div>
		</div>
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
@import url("https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@200;300;400;500;600;700;800&display=swap");

#fixex-menu-container {
	// border: 1px solid black;
	display: flex;
	flex-direction: row-reverse;
	width: 100px;
	position: fixed;
	right: 0;
	top: 12rem;
	
	#fixed-menu {
		// border: 1px solid red;
		height: 150px;
		width: 45px;
		display: flex;
		flex-direction: column;
		align-items: center;
		font-size: 1rem;
		justify-content: space-between;
		padding: 8px 0;
		background-color: white;
		border-top-left-radius: 5px;
		border-bottom-left-radius: 5px;
		box-shadow:  2px 2px 10px lightgray, -2px -2px 10px lightgray;

		i {
			color: #696969;
			cursor: pointer;
			transition: .2s ease-in-out;

			&:hover {
				color: #20ad96;
			}
		}
	}
}


</style>
