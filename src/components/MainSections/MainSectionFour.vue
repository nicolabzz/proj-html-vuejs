<template>
	<!-- Fourth section -->
	<main>
		<div class="cards-container">
			<div class="result-card">
				<h3>Successfully trained</h3>
				<h1>1790</h1>
				<span>ENROLLED LEARNERS</span>
			</div>
			<div class="result-card"></div>
			<div class="result-card"></div>
			<div class="result-card"></div>
		</div>
	</main>
</template>

<script>
export default {
	name: "MainSectionFour",
};
</script>

<style scoped lang="scss">
@import "../../css/global.scss";

.cards-container {
	border: 2px solid palevioletred;
	width: 1150px;
	margin: auto;
	height: 410px;
	display: flex;
	
	.result-card {
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
}
</style>