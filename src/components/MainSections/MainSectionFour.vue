<template>
	<!-- Fourth section -->
	<main>
		<div class="cards-container">
			<!-- <CardStatsMS4
				v-for="objCard in arrStats"
				:key="objCard.id"
				:title="objCard.titleText"
				:number="objCard.achivedNumbers"
				:what="objCard.textSubject"
				class="card-statistic"
			/> -->
			<div class="stats-card">
				<div class="title">
					<h3>Successfully trained</h3>
				</div>
				<h1>1790</h1>
				<span>ENROLLED LEARNERS</span>
			</div>
			<div class="stats-card">
				<div class="title">
					<h3>Proudly Recived</h3>
				</div>
				<h1>19</h1>
				<span>COUNTRYWIDE AWARDS</span>
			</div>
			<div class="stats-card">
				<div class="title">
					<h3>Firmly Established</h3>
				</div>
				<h1>24</h1>
				<span>LOCAL BRANCHES</span>
			</div>
			<div class="stats-card">
				<div class="title">
					<h3>Getting Featured on</h3>
				</div>
				<h1>1090</h1>
				<span>BLOG POST</span>
			</div>
		</div>
	</main>
</template>

<script>
// import CardStatsMS4 from "../Cards-Cycling/CardStatsMS4.vue";

export default {
	name: "MainSectionFour",
	components: {
		// CardStatsMS4,
	},
	data() {
		return {
			arrStats: [
				{
					titleText: "Successfully trained",
					achivedNumbers: 1790,
					textSubject: "ENROLLED LEARNERS",
				},
				{
					titleText: "Proudly Recived",
					achivedNumbers: 19,
					textSubject: "COUNTRYWIDE AWARDS",
				},
				{
					titleText: "Firmly Established",
					achivedNumbers: 24,
					textSubject: "LOCAL BRANCHES",
				},
				{
					titleText: "Getting Featured on",
					achivedNumbers: 1090,
					textSubject: "BLOG POST",
				},
			],
		};
	},
};
</script>

<style scoped lang="scss">
@import "../../css/global.scss";

.cards-container {
	// border: 2px solid palevioletred;
	width: 1150px;
	margin: auto;
	height: 410px;
	display: flex;

	

	.stats-card {
		// border: 1px solid goldenrod;
		border-left: .1px solid rgb(243, 243, 243);
		width: calc(100% / 4);
		height: 100%;
		display: flex;
		flex-direction: column;
		// align-items: center;
		text-align: center;
		justify-content: center;
		gap: 1.5rem;

		.title {
			// border: 1px solid goldenrod;
			// width: 20%;
			padding: 0 3rem;
			text-align: center;
		}

		h3 {
			color: #3f3a64;
			// word-spacing: 2rem;
			line-height: 2.3rem;
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

		&:last-child {
		border-right: .1px solid rgb(243, 243, 243);
		
		}
	}
}
</style>