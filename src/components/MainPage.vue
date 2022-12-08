<template>
	<!--
    The main'site pages is divided in "5" section, one above the other, I've call them:
    -First sections
    -Second section
    -Third section
    -Fourth section
    -Fourth sections
-->
	<div>
		<MainSectionOne />
		<MainSectionTwo />
		<MainSectionThree />
		<MainSectionFour />
		<MainSectionFive />
	</div>
</template>

<script>
import MainSectionOne from "./MainSections/MainSectionOne.vue";
import MainSectionTwo from "./MainSections/MainSectionTwo.vue";
import MainSectionThree from "./MainSections/MainSectionThree.vue";
import MainSectionFour from "./MainSections/MainSectionFour.vue";
import MainSectionFive from "./MainSections/MainSectionFive.vue";

export default {
	name: "MainPage",
	components: {
		MainSectionOne,
		MainSectionTwo,
		MainSectionThree,
		MainSectionFour,
		MainSectionFive,
	},
};
</script>

<style lang="scss" scoped>
@import "../css/global.scss";
</style>