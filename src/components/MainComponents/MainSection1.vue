<template>
	<!-- First section -->
	<main>
		<section class="first-section">
			<!-- This div sets the first section's max width -->
			<div class="firs-max-container">
				<!-- Title -->
				<div class="firs-title">
					<h5>SIMULATED TO LEARN?</h5>
					<h1>Featured Online Courses</h1>
				</div>

				<!-- Lessions Cards -->
				<div class="lessions-cards">
					<div class="card"></div>
				</div>

				<!-- Button "all courses" -->
				<div class="view-all-courses">
					<button></button>
				</div>
			</div>
		</section>
	</main>
</template>

<script>
export default {
	name: "MainSection1",
};
</script>

<style scoped lang="scss">
@import url(../css/global.scss);

.firs-max-container {
	border: 2px solid yellow;
	width: 1150px;
	height: 950px;
	margin: auto;
	font-family: "Inter", sans-serif;

	.firs-title {
		border: 2px solid pink;
		width: 100%;
		height: 20%;
		display: flex;
		align-items: center;
		justify-content: center;
		flex-direction: column;
		gap: 1rem;

		h5 {
			color: #aeadae;
			letter-spacing: 1px;
		}

		h1 {
			color: #3f3a64;
		}
	}

	.lessions-cards {
		border: 2px solid palevioletred;
		width: 100%;
		height: 70%;
	}
}
</style>