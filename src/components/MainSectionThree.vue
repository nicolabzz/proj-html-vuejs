<template>
	<!-- Third section -->
	<main>
		<!-- Text -->
		<div class="tile">
			<h4>GREAT WORDS ABOUT MAXCOACH</h4>
			<h1>Our <span>top learners'</span> verbatim</h1>
		</div>

		<!-- Testimonials cards -->
		<div class="testimonials-cards-container">
			<!-- Cards -->
			<div class="testimonial-card">
				<div class="testimonial-text">
					<h3>High level of efficency and scientific teaching methods</h3>
					<p>
						I am free ro learn at my own peace, fllow my own schedule and choose
						the subject I want to learn from the syllabus. Great study portal
						for people like me.
					</p>
				</div>
				<div class="testimonial-pic-n-name">
					<div class="testimonial-pic">
						<img src="../assets/img/testimonial-avata-02.jpg" alt="" />
					</div>
					<div class="testimonial-name">
						<h4>MINA HOLLACE</h4>
						<p>/ Freelancer</p>
					</div>
				</div>
			</div>
		</div>

		<!-- Start today section -->
		<div class="start-today-container">
			<div class="start-today">
				<h2>Start today getting <span>Online Certification</span></h2>
				<h1>You can be your own guiding star with our help!</h1>
				<button>Get started now</button>
			</div>
		</div>
	</main>
</template>

<script>
export default {
	name: "MainSectionThree",
};
</script>

<style scoped lang="scss">
@import "../css/global.scss";
main {
	background-color: #f8f8f8;
}

.tile {
	border: 2px solid purple;
	margin-top: 16rem;
	text-align: center;

	h4 {
		color: #696969;
		font-weight: 400;
		letter-spacing: 2px;
		margin-bottom: 1.5rem;
	}

	h1 {
		color: #3f3a64;

		span {
			color: #25ab94;
			font-weight: 400;
		}
	}
}

.testimonials-cards-container {
	margin-top: 4rem;
	// border: 2px solid goldenrod;
	height: 550px;

	.testimonial-card {
		// border: 2px solid blue;
		border-radius: 8px;
		height: 350px;
		width: 550px;
		padding: 2rem;
		background-color: white;

		.testimonial-text {
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

		.testimonial-pic-n-name {
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
				}

				p {
					color: #696969;
					font-weight: 500;
				}
			}
		}
	}
}

.start-today-container {
	// border: 2px solid yellowgreen;
	width: 1150px;
	height: 300px;
	margin: auto;
	display: flex;
	justify-content: center;
	text-align: center;
	// align-items: center;

	.start-today {
		// border: 2px solid blue;
		padding: 2.3rem 0 0 0;

		h2 {
			color: #3f3a64;
			letter-spacing: 1px;

			span {
				color: #25ab94;
				font-weight: 400;
			}
		}

		h1 {
			color: #3f3a64;
			margin-bottom: 2rem;
		}

		button {
			background-color: #25ab94;
			border: none;
			color: white;
			padding: 1rem 5rem;
			border-radius: 4px;
			font-weight: 800;
			transition: 0.2s ease-in-out;

			&:hover {
				background-color: #3f3a64;
				cursor: pointer;
			}
		}
	}
}
</style>