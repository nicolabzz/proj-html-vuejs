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
					<div class="card">
						<div class="card-pic">
							<img src="../assets/img/course-02-480x298.jpg" alt="" />
						</div>
						<div class="card-text">
							<p>$40.00</p>
							<h3>Learning to Write as a Professional Author</h3>
							<span><i class="fa-solid fa-sheet-plastic"></i> 20 Lessons</span>
							<span><i class="fa-regular fa-user"></i> 50 Students</span>
						</div>
					</div>
					<!-- <div class="card">
						<div class="card-pic">
							<img src="../assets/img/course-02-480x298.jpg" alt="" />
						</div>
						<div class="card-text">
							<p>$40.00</p>
							<h3>Learning to Write as a Professional Author</h3>
							<span><i class="fa-solid fa-sheet-plastic"></i> 20 Lessons</span>
							<span><i class="fa-regular fa-user"></i> 50 Students</span>
						</div>
					</div>
					<div class="card">
						<div class="card-pic">
							<img src="../assets/img/course-02-480x298.jpg" alt="" />
						</div>
						<div class="card-text">
							<p>$40.00</p>
							<h3>Learning to Write as a Professional Author</h3>
							<span><i class="fa-solid fa-sheet-plastic"></i> 20 Lessons</span>
							<span><i class="fa-regular fa-user"></i> 50 Students</span>
						</div>
					</div>
					<div class="card">
						<div class="card-pic">
							<img src="../assets/img/course-02-480x298.jpg" alt="" />
						</div>
						<div class="card-text">
							<p>$40.00</p>
							<h3>Learning to Write as a Professional Author</h3>
							<span><i class="fa-solid fa-sheet-plastic"></i> 20 Lessons</span>
							<span><i class="fa-regular fa-user"></i> 50 Students</span>
						</div>
					</div>
					<div class="card">
						<div class="card-pic">
							<img src="../assets/img/course-02-480x298.jpg" alt="" />
						</div>
						<div class="card-text">
							<p>$40.00</p>
							<h3>Learning to Write as a Professional Author</h3>
							<span><i class="fa-solid fa-sheet-plastic"></i> 20 Lessons</span>
							<span><i class="fa-regular fa-user"></i> 50 Students</span>
						</div>
					</div>
					<div class="card">
						<div class="card-pic">
							<img src="../assets/img/course-02-480x298.jpg" alt="" />
						</div>
						<div class="card-text">
							<p>$40.00</p>
							<h3>Learning to Write as a Professional Author</h3>
							<span><i class="fa-solid fa-sheet-plastic"></i> 20 Lessons</span>
							<span><i class="fa-regular fa-user"></i> 50 Students</span>
						</div>
					</div> -->
				</div>

				<!-- Button "all courses" -->
				<div class="courses-btn">
					<button>View all courses <i class="fa-solid fa-arrow-right-long"></i></button>
				</div>
			</div>
		</section>
	</main>
</template>

<script>
export default {
	name: "MainSectionOne",
};
</script>

<style scoped lang="scss">
@import url(../css/global.scss);

main {
background-color: #F5F7FA;
}

.max-container {
	border: 2px solid yellow;
	width: 1150px;
	height: 950px;
	margin: auto;
	font-family: "Inter", sans-serif;

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

		.card {
			// border: 1px solid purple;
			width: calc(1150px / 2);
			height: 221px;
			display: flex;
			align-items: center;
			padding: 5px;

			.card-pic {
				// border: 1px solid orange;
				height: 180px;
				width: 180px;
				border-radius: 50%;
				overflow: hidden;

				img {
					object-fit: cover;
					width: 100%;
					height: 100%;
				}
			}

			.card-text {
				// border: 2px solid black;
				height: 100%;
				width: 70%;
				padding: 1rem 0 .6rem 1rem;

				p {
					font-size: 1.5rem;
					font-weight: bold;
					color: #20ad96;
				}

				h3 {
					color: #3f3a64;
					margin: 1.5rem 0;
				}

				span {
				color: #aeadae;

				i {
				margin-right: .5rem;
				}
				}

				span:last-child {
					padding-left: 2.5rem;
				}
			}
		}
	}

	.courses-btn {
		border: 1px solid red;
		height: 10%;
		display: flex;
		align-items: center;
		justify-content: center;

		button {
			padding: .8rem 2.8rem;
			border: none;
			background-color: #20AD96;
			color: white;
			font-family: "Inter", sans-serif;
			cursor: pointer;
			border-radius: 4px;
			font-weight: 600;
		}
	}
}
</style>