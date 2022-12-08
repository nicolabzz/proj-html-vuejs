<template>
	<!-- First section -->
	<main>
		<section class="first-section">
			<!-- This div sets the first section's max width -->
			<div class="max-container">
				<!-- Title -->
				<div class="title">
					<h5>SIMULATED TO LEARN?</h5>
					<h1>Featured Online Courses</h1>
				</div>

				<!-- Lessions Cards -->
				<div class="lessions-cards-container">
					<CardCoursesMS1
						v-for="objCard in arrOnlineCourses"
						:key="objCard"
						:imgPic="objCard.imgSrc"
						:cost="objCard.price"
						:title="objCard.text"
						:info1="objCard.lessions"
						:info2="objCard.students"
						class="CardCourse"
					/>
				</div>

				<!-- Button "all courses" -->
				<div class="courses-btn">
					<button>
						View all courses <i class="fa-solid fa-arrow-right-long"></i>
					</button>
				</div>
			</div>
		</section>
	</main>
</template>

<script>
import CardCoursesMS1 from "../Cards-Cycling/CardCoursesMS1.vue";

export default {
	name: "MainSectionOne",
	components: {
		CardCoursesMS1,
	},
	data() {
		return {
			arrOnlineCourses: [
				{
					imgSrc: 'img/course-02-480x298.jpg',
					price: '$40.00',
					text: 'Learning to Write as a Professional Author',
					lessions: ' 20 Lessons',
					students: ' 50 Students',
				},
				{
					imgSrc: 'img/stock-full-hd-03-480x298.jpg',
					price: 'Free',
					text: 'Costumer-centric Info-Tech Strangers',
					lessions: ' 24 Lessons',
					students: ' 769 Students',
				},
				{
					imgSrc: 'img/stock-full-hd-04-480x298.jpg',
					price: '$19.00',
					text: 'Open Programming Courses for Everyone:Python',
					lessions: ' 17 Lessons',
					students: ' 62 Students',
				},
				{
					imgSrc: 'img/stock-full-hd-06-480x298.jpg',
					price: '$26.00',
					text: 'Accademic Listening and Note-taking',
					lessions: ' 14 Lessons',
					students: ' 67 Students',
				},
				{
					imgSrc: 'img/course-featured-image-01-480x298.jpg',
					price: '$39.00',
					text: 'Master jQuery in a Short Period of Time',
					lessions: ' 6 Lessons',
					students: ' 51 Students',
				},
				{
					imgSrc: 'img/stock-full-hd-05-480x298.jpg',
					price: '$59.00',
					text: 'Introduction to Javascript for Beginners',
					lessions: ' 14 Lessons',
					students: ' 76 Students',
				},
			],
		};
	},
};
</script>

<style scoped lang="scss">
@import "../../css/global.scss";

main {
	background-color: #f5f7fa;
}

.max-container {
	border: 2px solid yellow;
	width: 1150px;
	height: 950px;
	margin: auto;

	.title {
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
			font-size: 2rem;
		}
	}

	.lessions-cards-container {
		border: 2px solid palevioletred;
		width: 100%;
		height: 70%;
		display: flex;
		flex-wrap: wrap;

		.CardCourse {
		flex: 0 0 50%;
		}
	}

	.courses-btn {
		border: 1px solid red;
		height: 10%;
		display: flex;
		align-items: center;
		justify-content: center;

		button {
			padding: 0.8rem 2.8rem;
			border: none;
			background-color: #20ad96;
			color: white;
			cursor: pointer;
			border-radius: 4px;
			font-weight: 600;
			transition: 0.2s ease-in-out;

			&:hover {
				background-color: #3f3a64;
				cursor: pointer;
			}
		}
	}
}
</style>