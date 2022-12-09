<template>
	<!-- Third section -->
	<main>
		<!-- Text -->
		<div class="tile">
			<h4>GREAT WORDS ABOUT MAXCOACH</h4>
			<h1>Our <span>top learners'</span> verbatim</h1>
		</div>

		<!-- Testimonials cards section -->
		<div class="testimonials-cards-container">
			<!-- Cards -->
			<CardReviewMS3
				v-for="objTestimonial in arrTestimonials"
				:key="objTestimonial.id"
				:title="objTestimonial.titleT"
				:text="objTestimonial.textT"
				:imgPic="objTestimonial.imgSrcT"
				:name="objTestimonial.nameT"
				:job="objTestimonial.jobT"
			/>

			<div class="selector">
				<span><i class="fa-solid fa-circle"></i></span>
				<span><i class="fa-solid fa-circle"></i></span>
				<span><i class="fa-solid fa-circle"></i></span>
				<span><i class="fa-solid fa-circle"></i></span>
			</div>
		</div>

		<!-- Button section -->
		<div class="btn-container">
			<div class="det1">
				<img src="img/maxcoach-shape-01.png" alt="">
			</div>
			<div class="dit2">
				<img src="img/gray-circle.png" alt="">
			</div>
			<div class="dit3">
				<img src="img/maxcoach-shape-02.png" alt="">
			</div>
			<div class="start-today">
				<h2>Start today getting <span>Online Certification</span></h2>
				<h1>You can be your own guiding star with our help!</h1>
				<button>Get started now</button>
			</div>
		</div>
	</main>
</template>

<script>
import CardReviewMS3 from "../Cards-Cycling/CardReviewMS3.vue";

export default {
	name: "MainSectionThree",
	components: {
		CardReviewMS3,
	},
	data() {
		return {
			arrTestimonials: [
				{
					titleT: "It's a choice of quality for people with special needs",
					textT:
						"I'm very strict person so I requiire everything to be organized and neat. Then, I'll be able to make things right and shine. MaxCoach guys just got me.",
					imgSrcT: "img/testimonial-avata-03.jpg",
					nameT: "FLORENCE THEMES",
					jobT: "/ Multimedia Admin",
				},
				{
					titleT: "High level of efficency and scientific teaching methods",
					textT:
						"I am free ro learn at my own peace, fllow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.",
					imgSrcT: "img/testimonial-avata-02.jpg",
					nameT: "MINA HOLLACE",
					jobT: "/ Freelancer",
				},
				{
					titleT:
						"Professional team of specialist and passionate metors at reach",
					textT:
						"I need to get a certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students with students.",
					imgSrcT: "img/testimonial-avata-04.jpg",
					nameT: "MADLEY PONDOR",
					jobT: "/ IT Specialist",
				},
			],
		};
	},
};
</script>

<style scoped lang="scss">
@import "../../css/global.scss";

main {
	background-color: #f8f8f8;
	// border: 2px solid black;
}

//Title section
.tile {
	// border: 2px solid purple;
	padding-top: 5rem;
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

//Center section (Testimonial cards)
.testimonials-cards-container {
	// border: 2px solid goldenrod;
	margin-top: 2rem;
	height: 480px;
	display: flex;
	justify-content: space-between;
	flex-wrap: wrap;
	padding: 0 2rem;

	.selector {
		// border: 2px solid brown;
		width: 700px;
		margin: auto;
		height: 50px;
		display: flex;
		justify-content: center;
		align-items: center;
		gap: 1.5rem;
		
		i {
			color: #B7B5C4;
			font-size: .75rem;
			transition: .1s ease-in;
			scale: (1);

			&:hover {
				scale: (1.2);
				cursor: pointer;
				color: #3F3A64;
			}
		}
	}
}

//Button sectoion
.btn-container {
	// border: 2px solid yellowgreen;
	width: 1150px;
	height: 300px;
	margin: auto;
	display: flex;
	justify-content: center;
	text-align: center;
	position: relative;
	// align-items: center;

	.det1 {
	position: absolute;
	// height: 100px;
	// width: 100px;
	left: 0;
	top: 50%;
	}
	.dit2 {
		position: absolute;
		height: 80px;
		width: 80px;
		left: 0;
		top: 5%;
	}
	.dit3 {
		position: absolute;
		right: 0;
		bottom: 15%;
	}

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