<!-- <template>
	<div class="stats-card">
		<h3>{{ title }}</h3>
		<h1>{{ number }}</h1>
		<span>{{ what }}</span>
	</div>
</template>

<script>
export default {
	name: "CardStatsMS4",
	props: {
		title: String,
		number: String,
		what: String,
	},
};
</script>

<style lang="less" scoped>
@import "../../css/global.scss";

.stats-card {
	border: 1px solid goldenrod;
	width: calc(100% / 4);
	height: 100%;
	display: flex;
	flex-direction: column;
	// align-items: center;
	text-align: center;
	justify-content: center;
	gap: 1.5rem;

	h3 {
		color: #3f3a64;
		word-spacing: 2rem;
		line-height: 2rem;
		font-size: 1.6rem;
		font-weight: 800;
	}

	h1 {
		color: #20ad96;
		font-size: 3.5rem;
		font-weight: 900;
	}

	span {
		color: #8c89a2;
		font-weight: 800;
		letter-spacing: 2px;
	}
}
</style> -->