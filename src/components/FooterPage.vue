<template>
	<!--
  The Footer is divided in "2" sections, one abive the other, "Footer Top" n "Footer Bottom"
-->
	<footer>
		<!-- Footer top -->
		<div class="top-section">
			<!-- This div sets the max width for the contents -->
			<div class="top-max-container">
				<!-- Contents -->
				<div class="subscribe-text">
					<h1>Subscribe <span>Newsletters</span></h1>
					<p>
						Enter your email address to register to our newsletter subscroption
						delivered on a regular basis!
					</p>
				</div>
			</div>
		</div>

		<!-- ============================================== -->

		<!-- Footer bottom -->
		<div class="bottom-section">
			<!-- This div sets the max width for the contents -->
			<div class="bottom-max-container">
				<!--  Links -->
				<div class="links-section">
					<div class="address"></div>
					<div class="social"></div>

					<div class="explore-information"></div>

					<!-- Rights Reserved -->
					<div class="right-reserved"></div>
				</div>
			</div>
		</div>
	</footer>
</template>

<script>
export default {
	name: "FooterPage",
};
</script>

<style scoped lang="scss">
@import "../css/global.scss";

footer {
	height: 820px;
}

.top-section {
	border: 1px solid firebrick;
	height: 410px;

	.top-max-container {
		border: 1px solid firebrick;
		width: 1150px;
		height: 100%;
		margin: auto;
	}
}

.bottom-section {
	border: 1px solid firebrick;
	height: 410px;

	.bottom-max-container {
		border: 1px solid firebrick;
		width: 1150px;
		height: 100%;
		margin: auto;
	}
}

.subscribe-text {
border: 2px solid lightblue;
text-align: center;

h1 {
color: #3F3A64;

span {

}
}
}
</style>