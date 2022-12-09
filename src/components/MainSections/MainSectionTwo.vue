<template>
	<div class="big-cont">
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

					<!-- Cards smart tutoring course's benefits -->
					<div class="benefits-cards-container">
						<CardBenefitsMS2
							v-for="objCard in arrSmartTutoring"
							:key="objCard.id"
							:imgPic="objCard.imgSrc"
							:title="objCard.textTitle"
							:content="objCard.textContent"
							:link="objCard.textLink"
							class="CardBenefits"
						/>
					</div>

					<!-- "YouTube video" and "enjoy" section -->
					<div class="yt-n-enjoy-container">
						<!-- YouTube video container -->
						<div class="ytv-section">
							<!-- YT Video -->
							<div class="video-section">
								<div class="logo">
									<img src="img/icon-youtube-play.png" alt="" />
								</div>
							</div>
						</div>

						<!-- Enjoy container-->
						<div class="enjoy-container">
							<div class="details-container">
								<div class="details-img-section">
									<img src="img/rose-circle.png" alt="" />
								</div>
							</div>
							<div class="enjoy-text">
								<h4>GET STARTED <span>EFFORTLESSY</span></h4>
								<h1>Enjoy Our <span>Companionship</span></h1>
								<p>
									Sneek peek into what has in store for you on our online
									teaching and mentoring portal. Seek for some hidden hints of
									early-bird rewards as well.
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
	</div>
</template>

<script>
import CardBenefitsMS2 from "../Cards-Cycling/CardBenefitsMS2.vue";

export default {
	name: "MainSectionTwo",
	components: {
		CardBenefitsMS2,
	},
	data() {
		return {
			arrSmartTutoring: [
				{
					imgSrc: "img/home-2-image-box-01.png",
					textTitle: "Costumize Preferences",
					textContent:
						"Learners are given the right to arrange and costumize their study schedule and timetable based on preferences.",
					textLink: "Start Here",
				},
				{
					imgSrc: "img/about-us-02-image-box-02.png",
					textTitle: "Cloud Storage",
					textContent:
						"You can store online lessons via online cloud or download to your device and revise lessions on the way.",
					textLink: "Get Free Quote",
				},
				{
					imgSrc: "img/home-2-image-box-03.png",
					textTitle: "Multimedia Channels",
					textContent:
						"We provide study materials with various formats: video, audio, slides, doc, prints, books and applications.",
					textLink: "Start Here",
				},
			],
		};
	},
};
</script>

<style scoped lang="scss">
@import "../../css/global.scss";

.big-cont {
	background-color: #f8f8f8;
}

main {
	// border: 2px solid black;
	background-color: white;
	border-bottom-right-radius: 40%;
	height: 1400px;
}

.max-container {
	// border: 2px solid black;
	width: 1375px;
	height: 1400px;
	margin: 0 auto;
	margin-bottom: 2rem;

	// Title section
	.title {
		// border: 2px solid cadetblue;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		height: 15%;
		color: #3f3a64;
		gap: 15px;

		h4 {
			color: #9795ab;
			// font-size: 1.5rem;
			font-weight: 500;
			letter-spacing: 1px;
		}

		h1 {
			color: #3f3a64;
			font-size: 1.7rem;

			span {
				color: #20ad96;
				font-weight: 400;
			}
		}
	}

	// Carde course Bnefits
	.benefits-cards-container {
		// border: 2px solid cadetblue;
		margin: 0 auto;
		display: flex;
		width: 1000px;
		height: 25%;

		.CardBenefits {
			flex: 0 0 33.33333333333%;
		}
	}

	//Bottom section w/ YT video
	.yt-n-enjoy-container {
		// border: 2px solid cadetblue;
		height: 50%;
		width: 100%;
		display: flex;

		.ytv-section {
			// border: 2px solid palevioletred;
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
				background-image: url(../../../public/img/home-2-popup-video-poster.jpg);
				z-index: 0;
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
			// border: 2px solid palevioletred;
			width: 40%;
			display: flex;
			align-items: center;
			justify-content: center;
			flex-direction: column;

			.details-container {
				// border: 2px solid blue;
				width: 100%;
				
				.details-img-section {
					// border: 2px solid yellow;
					width: 100px;
					height: 100px;
					margin-left: 1rem;

					img {
					}
				}
			}

			.enjoy-text {
				// border: 2px solid goldenrod;
				width: 100%;
				padding: 0 2.6rem;

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
					// border-bottom: 1px solid lavender;
					color: #25ab94;
					font-weight: 700;
				}
			}
		}
	}
}
</style>