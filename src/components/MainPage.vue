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
import MainSectionOne from "./MainSectionOne.vue";
import MainSectionTwo from "./MainSectionTwo.vue";
import MainSectionThree from "./MainSectionThree.vue";
import MainSectionFour from "./MainSectionFour.vue";
import MainSectionFive from "./MainSectionFive.vue";

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
@import url(../css/global.scss);
</style>