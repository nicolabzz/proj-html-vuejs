<template>
	<div class="testimonial-card">
		<div class="testimonial-text-content">
			<h3>{{title}}</h3>
			<p>{{text}}</p>
		</div>
		<div class="testimonial-info">
			<div class="testimonial-pic">
				<img :src="imgPic" alt="" />
			</div>
			<div class="testimonial-name">
				<h4>{{name}}</h4>
				<p>{{job}}</p>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "CardReviewMS3",
	props: {
		title: String,
		text: String,
		imgPic: String,
		name: String,
		job: String,
	},
};
</script>

<style scoped lang="scss">

.testimonial-card {
		// border: 2px solid black;
		border-radius: 8px;
		height: 380px;
		width: 550px;
		padding: 2rem;
		background-color: white;

		.testimonial-text-content {
			// border: 2px solid blue;
			height: 60%;
			width: 100%;
			padding: 0 2rem;

			h3 {
				color: #3f3a64;
				margin-bottom: 1rem;
			}

			p {
				color: #696969;
				font-weight: 500;
				line-height: 2;
			}
		}

		.testimonial-info {
			// border: 2px solid salmon;
			display: flex;
			padding: 0 2rem;

			.testimonial-pic {
				width: 70px;
				height: 70px;
				border-radius: 50%;
				overflow: hidden;
			}

			.testimonial-name {
				display: flex;
				flex-direction: column;
				justify-content: space-between;
				padding: 0.7rem 2rem;

				h4 {
					margin-bottom: 1rem;
					color: #3f3a64;
					font-weight: 800;
          letter-spacing: 1px;
				}

				p {
					color: #9c9c9c;
					font-weight: 500;
          font-size: 13px;
				}
			}
		}
	}
</style>