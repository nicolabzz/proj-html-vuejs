<template>
	<!-- Second section -->
	<main>
		<section class="second-section">
			<!-- This div sets the second section's max width -->
			<div class="max-container">
				<!-- Title -->
				<div class="title">
					<h4>MAXCOACH AVAILABLE COURSES</h4>
					<h1>Access <span>Smart Tutoring</span> Program For Benefits.</h1>
				</div>

				<!-- Cards course's benefits -->
				<div class="benefits-cards-container">
					<div class="card">
						<div class="card-pic">
							<img src="../assets/img/home-2-image-box-01.png" alt="" />
						</div>
						<div class="card-text">
							<h3>Costumize Preferences</h3>
							<p>
								Learners are given the right to arrange and costumize their
								study schedule and timetable based on preferences.
							</p>
							<a href="https://www.youtube.com/watch?v=dQw4w9WgXcQ"
								>Start Here <i class="fa-solid fa-arrow-right-long"></i
							></a>
						</div>
					</div>
					<div class="card"></div>
					<div class="card"></div>
				</div>

				<!-- "YouTube video" and "enjoy" section -->
				<div class="yt-n-enjoy-container">
					<!-- YouTube video container -->
					<div class="ytv-section">
						<!-- YT Video -->
						<div class="video-section">
							<div class="logo">
								<img src="../assets/img/icon-youtube-play.png" alt="" />
							</div>
						</div>
					</div>

					<!-- Enjoy container-->
					<div class="enjoy-container">
						<div class="enjoy-text">
							<h4>GET STARTED <span>EFFORTLESSY</span></h4>
							<h1>Enjoy Our <span>Companionship</span></h1>
							<p>
								Sneek peek into what has in store for you on our online teaching
								and mentoring portal. Seek for some hidden hints of early-bird
								rewards as well.
							</p>
							<a href=""
								>Download free guidebook
								<i class="fa-solid fa-arrow-right-long"></i
							></a>
						</div>
					</div>
				</div>
			</div>
		</section>
	</main>
</template>

<script>
export default {
	name: "MainSectionTwo",
};
</script>

<style scoped lang="scss">
@import "../css/global.scss";

.max-container {
	border: 2px solid black;
	width: 1375px;
	height: 1100px;
	margin: auto;

	.title {
		border: 2px solid cadetblue;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		height: 15%;
		color: #3f3a64;
		gap: 15px;

		h4 {
			color: #9795ab;
		}

		h1 {
			color: #3f3a64;

			span {
				color: #25ab94;
				font-weight: 400;
			}
		}
	}
	.benefits-cards-container {
		border: 2px solid cadetblue;
		margin: 0 auto;
		display: flex;
		width: 1150px;
		height: 35%;

		.card {
			border: 2px solid greenyellow;
			width: calc(100% / 3);

			.card-pic {
				border: 2px solid salmon;
				height: 50%;
				width: 100%;

				img {
					height: 100%;
					object-fit: contain;
					object-position: left;
					scale: 0.87;
				}
			}

			h3 {
				color: #3f3a64;
			}

			p {
				color: #9795ab;
				padding: 2rem 0;
				// font-size: .8rem;
			}
		}
	}

	.yt-n-enjoy-container {
		border: 2px solid cadetblue;
		height: 50%;
		width: 100%;
		display: flex;

		.ytv-section {
			border: 2px solid palevioletred;
			width: 60%;
			position: relative;

			.video-section {
				// border: 4px solid red;
				height: 490px;
				width: 700px;
				overflow: hidden;
				position: absolute;
				right: 20px;
				bottom: 20px;
				background-image: url(../assets/img/home-2-popup-video-poster.jpg);
				background-repeat: no-repeat;
				background-size: contain;
				display: flex;
				justify-content: center;
				align-items: center;
				border-radius: 5px;

				.logo {
					width: 100px;
					height: 100px;
				}
			}
		}

		.enjoy-container {
			border: 2px solid palevioletred;
			width: 40%;
			display: flex;
			align-items: center;
			justify-content: center;

			.enjoy-text {
				border: 2px solid goldenrod;
				width: 100%;
				padding: 0 3rem;

				h4 {
					color: #9795ab;
					margin-bottom: 2rem;

					span {
						color: #3f3a64;
					}
				}

				h1 {
					font-size: 3rem;
					margin-bottom: 1.5rem;
					color: #3f3a64;

					span {
						color: #25ab94;
						font-weight: 400;
					}
				}

				p {
					font-size: 1.5rem;
					color: #696969;
					font-weight: 300;
					font-weight: 400;
					margin-bottom: 3rem;
				}

				a {
					border-bottom: 1px solid lavender;
					color: #25ab94;
					font-weight: 700;
				}
			}
		}
	}
}
</style>