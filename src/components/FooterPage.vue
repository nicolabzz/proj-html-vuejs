<template>
	<!--
  The Footer is divided in "2" sections, one abive the other, "Footer Top" n "Footer Bottom"
-->
	<footer>
		<!-- Footer top -->
		<div class="top-section">
			<!-- This div sets the max width for the contents -->
			<div class="top-max-container">
				<div class="green-circle">
					<img src="img/green-circle.png" alt="" />
				</div>
				<div class="colored-lines">
					<img src="img/maxcoach-shape-02.png" alt="" />
				</div>
				<div class="details-grid">
					<img src="img/maxcoach-shape-09.png" alt="" />
				</div>
				<!-- Contents -->
				<div class="top-centering">
					<div class="subscribe-text">
						<h1>Subscribe <span>Newsletters</span></h1>
						<p>
							Enter your email address to register to our newsletter
							subscroption delivered on a regular basis!
						</p>
					</div>
					<div class="form-section">
						<input type="text" placeholder="Enter your email" />
						<button>Subscribe</button>
					</div>
				</div>
			</div>
		</div>

		<!-- ============================================== -->

		<!-- Footer bottom -->
		<div class="bottom-section">
			<!-- This div sets the max width for the contents -->
			<div class="bottom-max-container">
				<!--  Links -->
				<AddressLinksFooter :footerData="footerData" />

				<div class="explore-information">
					<ExploreLinksFooter :footerData="footerData" />

					<InformationLinksFooter :footerData="footerData" />

					<div class="information">
						<h3>Information</h3>
						<div id="col3">
							<a href="#">Membership</a>
							<a href="#">Purchase guide</a>
							<a href="#">Privacy policy</a>
							<a href="#">Terms of services</a>
						</div>
					</div>
				</div>

				<!-- Rights Reserved -->
				<div class="right-reserved">
					<p>
						<i class="fa-regular fa-copyright"></i> 2020 Maxcoach. All right
						Reserved
					</p>
				</div>
			</div>
			<div class="arrow-top-container">
				<div class="arrow-top">
					<span><i class="fa-solid fa-arrow-up-long"></i></span>
				</div>
			</div>
		</div>
	</footer>
</template>

<script>
import AddressLinksFooter from "@/components/Cards-Cycling/AddressLinksFooter.vue";
import ExploreLinksFooter from "@/components/Cards-Cycling/ExploreLinksFooter.vue";
import InformationLinksFooter from "@/components/Cards-Cycling/InformationLinksFooter.vue";

export default {
	name: "FooterPage",
	components: {
		AddressLinksFooter,
		ExploreLinksFooter,
		InformationLinksFooter,
	},
	data() {
		return {
			footerData: {
				// ADDRESS COLUMN
				addressCol: {
					linkTitle: "Address",
					location: "382 NE 191st St # 87394 Miami, FL 33179-3899",
					phone: "+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)",
					eMail: "support@maxcoach.com",
					social: [
						{
							socialLink: "fa-brands fa-square-facebook",
						},
						{
							socialLink: "fa-brands fa-twitter",
						},
						{
							socialLink: "fa-brands fa-instagram",
						},
						{
							socialLink: "fa-brands fa-linkedin",
						},
					],
				},
				//EXPLORE COLUMN
				exploreCol: {
					linkTitle: "Explore",
					links1: ["Start here", "Blog", "About us"],
					links2: ["Success story", "Courses", "Contuct us"],
				},
				//INFORMATION COLUMN
				informationCol: {
					linkTitle: "Information",
					links: [
						"Membership",
						"Purchase guide",
						"Privacy policy",
						"Terms of services",
					],
				},
			},
		};
	},
};
</script>

<style scoped lang="scss">
@import "../css/global.scss";

footer {
	height: 820px;
}

// Common
.top-section,
.bottom-section {
	// border: 1px solid firebrick;
	height: 410px;

	.top-max-container,
	.bottom-max-container {
		// border: 1px solid firebrick;
		width: 1150px;
		height: 100%;
		margin: auto;
	}
}

//Top FOOTER
.top-max-container {
	// border: 2px solid orange;
	display: flex;
	align-items: center;
	justify-content: center;
	position: relative;

	.green-circle {
		// border: 1px solid firebrick;
		width: 80px;
		height: 80px;
		overflow: hidden;
		position: absolute;
		left: 0;
		bottom: 25%;
	}
	.colored-lines {
		width: 135px;
		height: 135px;
		right: 0;
		bottom: 25%;
		overflow: hidden;
		position: absolute;
	}
	.details-grid {
		// border: 2px solid orange;

		width: 200px;
		height: 200px;
		right: 2rem;
		top: 6%;
		overflow: hidden;
		position: absolute;
	}

	.top-centering {
		// border: 2px solid orange;

		.subscribe-text {
			// border: 2px solid lightblue;
			text-align: center;
			margin: auto;
			width: 80%;
			margin-bottom: 3rem;

			h1 {
				color: #3f3a64;
				margin-bottom: 1rem;

				span {
					color: #20ad96;
					font-weight: 400;
				}
			}

			p {
				line-height: 2rem;
				color: #696969;
				font-weight: 500;
				font-size: 1.1rem;
			}
		}

		.form-section {
			display: flex;
			justify-content: center;

			input {
				border: none;
				background-color: #f5f5f5;
				height: 55px;
				width: 430px;
				border-top-left-radius: 3px;
				border-bottom-left-radius: 3px;
				padding-left: 1rem;
				font-weight: 500;
			}

			button {
				padding: 0 2rem;
				height: 55px;
				border: none;
				border-top-right-radius: 3px;
				border-bottom-right-radius: 3px;
				font-weight: 800;
				color: white;
				background-color: #20ad96;
				transition: 0.3s ease-in-out;

				&:hover {
					background-color: #3f3a64;
					cursor: pointer;
				}
			}
		}
	}
}

//Bottom FOOTER
.bottom-section {
	background-color: #f8f8f8;

	.bottom-max-container {
		// border: 1px solid violet;
		padding: 5rem 0 0 0;
		display: flex;
		flex-wrap: wrap;
	}

	.explore-information {
		// border: 2px solid rgb(0, 192, 99);
		height: 250px;
		width: 50%;
		display: flex;

		.information {
			// border: 2px solid violet;
			width: 50%;
			padding-top: 0.7rem;

			#col3 {
				// border: 1px solid black;
				line-height: 3rem;
				width: 50%;

				a {
					display: block;
					color: #696969;
					font-weight: 600;
					font-size: 13px;
					transition: 0.15s ease-in-out;

					&:hover {
						color: #20ad96;
					}
				}

				h3 {
					color: #333333;
				}
			}
		}
	}

	.right-reserved {
		// border: 2px solid salmon;
		width: 100%;
		text-align: center;

		p {
			font-size: 14px;
			color: #c3c3c3;
			font-weight: 600;
		}
	}
}

.arrow-top-container {
	// border: 2px solid blue;
	width: 100%;
	display: flex;
	flex-direction: row-reverse;
	padding: 0 1rem 0.5rem 0;
	background-color: #f8f8f8;

	.arrow-top {
		span {
			height: 50px;
			width: 50px;
			padding: 1.5rem;
			background-color: #20ad96;
			border-radius: 50%;
			display: flex;
			align-items: center;
			justify-content: center;
			cursor: pointer;
			transition: transform 1s ease-in-out;
			scale: (1);

			&:hover {
				transform: scale(1.1);
				transform: rotate(720deg);
				scale: (1.2);
				background-color: #3f3a64;
			}
			i {
				color: white;
			}
		}
	}
}
</style>