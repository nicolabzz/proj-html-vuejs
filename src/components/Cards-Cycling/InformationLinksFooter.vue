<template>
	<div class="information">
		<h3>{{ title }}</h3>
		<div id="col3">
			<a href="#">{{ linkOne }}</a>
			<a href="#">{{ linkTwo }}</a>
			<a href="#">{{ linkThree }}</a>
			<a href="#">{{ linkFour }}</a>
		</div>
	</div>
</template>

<script>
export default {
	name: "InformationLinksFooter",
	props: {
		title: String,
		linkOne: String,
		linkTwo: String,
		linkThree: String,
		linkFour: String,
	},
};
</script>

<style scoped lang="scss">
@import "../../css/global.scss";

.information {
	// border: 2px solid violet;
	width: 50%;
	padding-top: 0.7rem;

	#col3 {
		// border: 1px solid black;
		line-height: 3rem;
		width: 50%;

		a {
			display: block;
			color: #696969;
			font-weight: 600;
			font-size: 13px;
			transition: 0.15s ease-in-out;

			&:hover {
				color: #20ad96;
			}
		}

		h3 {
			color: #333333;
		}
	}
}
</style>