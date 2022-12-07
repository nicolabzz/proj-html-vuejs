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
				<div class="links-section">
					<div class="address">
						<h3>Address</h3>
						<p>382 NE 191st St # 87394 Miami, FL 33179-3899</p>
						<p>+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)</p>
						<p>support@maxcoach.com</p>
					</div>

					<div class="social">
						<a href=""><i class="fa-brands fa-square-facebook"></i></a>
						<a href=""><i class="fa-brands fa-twitter"></i></a>
						<a href=""><i class="fa-brands fa-instagram"></i></a>
						<a href=""><i class="fa-brands fa-linkedin"></i></a>
					</div>
				</div>

				<div class="explore-information">
					<div class="explore">
						<h3>Explore</h3>
						<div id="col1">
							<a href="#">Start here</a>
							<a href="#">Blog</a>
							<a href="#">About us</a>
						</div>
						<div id="col2">
							<a href="#">Success story</a>
							<a href="#">Courses</a>
							<a href="#">Contuct us</a>
						</div>
					</div>
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
	display: flex;
	align-items: center;
	justify-content: center;

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
				transition: .3s ease-in-out;
				
				&:hover {
					background-color: #3F3A64;
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
		padding: 3.2rem 0;
		display: flex;
		flex-wrap: wrap;
	}

	.links-section {
		// border: 2px solid blue;
		height: 250px;
		width: 50%;
		line-height: 3rem;

		.address {
			h3 {
				color: #333333;
			}

			p {
				color: #696969;
				font-weight: 600;
				font-size: 0.86rem;
			}
		}

		.social {
			font-size: 1.5rem;
			margin: 1rem 0 0 0;
			width: 40%;
			display: flex;
			justify-content: space-between;

			a {
				color: #b1b1b1;
			}
		}
	}

	.explore-information {
		// border: 2px solid rgb(0, 192, 99);
		height: 250px;
		width: 50%;
		display: flex;

		.explore {
			// border: 2px solid rgb(60, 213, 224);
			width: 50%;
			padding-top: 0.7rem;

			h3 {
				color: #333333;
				width: 100%;
			}

			#col1 {
				// border: 1px solid black;
				display: inline-block;
				line-height: 3rem;
				width: 50%;
			}
			#col2 {
				// border: 1px solid black;
				display: inline-block;
				line-height: 3rem;
				width: 50%;
			}

			a {
				display: block;
				color: #696969;
				font-weight: 600;
				font-size: 13px;
			}
		}

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
			font-size: 12px;
			color: #696969;
			font-weight: 600;
		}
	}
}
</style>