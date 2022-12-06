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
		<MainSection1 />
		<MainSection2 />
		<MainSection3 />
		<MainSection4 />
		<MainSection5 />
	</div>
</template>

<script>
import MainSection1 from "./MainComponents/MainSection1.vue";
import MainSection2 from "./MainComponents/MainSection2.vue";
import MainSection3 from "./MainComponents/MainSection3.vue";
import MainSection4 from "./MainComponents/MainSection4.vue";
import MainSection5 from "./MainComponents/MainSection5.vue";

export default {
	name: "MainPage",
	components: {
		MainSection1,
		MainSection2,
		MainSection3,
		MainSection4,
		MainSection5,
	},
};
</script>

<style lang="scss" scoped>
@import url(../css/global.scss);

</style>