<template>
	<div class="explore">
		<h3>{{ footerData.exploreCol.linkTitle }}</h3>
		<div id="col1">
			<a v-for="link in footerData.exploreCol.links1" :key="link" href="#">
				{{ link }}
			</a>
		</div>
		<div id="col2">
			<a v-for="link in footerData.exploreCol.links2" :key="link" href="#">
				{{ link }}
			</a>
		</div>
	</div>
</template>

<script>
export default {
	name: "ExploreLinksFooter",
	props: {
		footerData: Object,
	},
};
</script>

<style scoped lang="scss">
@import "../../css/global.scss";

.explore {
	// border: 2px solid rgb(60, 213, 224);
	width: 50%;
	padding-top: 0.7rem;

	h3 {
		color: #333333;
		width: 100%;
	}

	#col1 {
		// border: 1px solid black;
		display: inline-block;
		line-height: 3rem;
		width: 50%;
	}
	#col2 {
		// border: 1px solid black;
		display: inline-block;
		line-height: 3rem;
		width: 50%;
	}

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
}
</style>