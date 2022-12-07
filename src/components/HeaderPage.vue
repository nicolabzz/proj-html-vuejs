<template>
	<!--
    The header is divided in 2 sections, one above the other, the "header-top" and the "header-bottom"
-->
	<header>
		<div class="container-top">
			<!-- Top section -->
			<section class="header-top">
				<!-- Logo -->
				<div class="logo">
					<img src="../assets/img/dark-logo.png" alt="" />
				</div>

				<!-- Nav options -->
				<div class="nav-section">
					<nav>
						<a href="">Home<i class="fa-solid fa-chevron-down"></i></a>
						<a href="">Pages<i class="fa-solid fa-chevron-down"></i></a>
						<a href="">Courses<i class="fa-solid fa-chevron-down"></i></a>
						<a href="">Features<i class="fa-solid fa-chevron-down"></i></a>
						<a href="">Blog<i class="fa-solid fa-chevron-down"></i></a>
						<a href="">Shop<i class="fa-solid fa-chevron-down"></i></a>
					</nav>

					<!-- Account -->
					<div class="account">
						<i class="fa-regular fa-circle-user"></i>
					</div>

					<!-- Search bar -->
					<span class="search-section">
						<input type="text" id="searchbar" placeholder="Search..." />
						<i class="fa-solid fa-magnifying-glass"></i>
					</span>
				</div>
			</section>
		</div>

		<!-- This div sets the container's max with -->
		<div class="container-bottom">
			<!-- Text presentation -->
			<div class="text-presentation-container">
				<div class="text-section">
					<div class="text-box">
						<h1>Distant learning for further expansion</h1>
						<p>
							Learning is a life-long journey that in fact we never find the
							terminate stop. Stop searching, enjoy the process.
						</p>
					</div>

					<div class="button-download">
						<button>
							<i class="fa-solid fa-download"></i>
							Download free guide
						</button>
					</div>

					<div class="free-sample">
						<p>
							Have a quwstion?
							<span>
								Get Free Sample <i class="fa-solid fa-arrow-right-long"></i>
							</span>
						</p>
					</div>
				</div>
			</div>

			<!-- Big Pic -->
			<div class="big-pic-presentation">
				<div class="img-fitter">
					<img
						src="../assets/img/about-me-profile-ohm4dxoearqbxny7q3bq1pzbdgofdx0tobbeqcvzd0.jpg"
						alt=""
					/>
				</div>
			</div>

			<!-- Clients Logos -->
			<div class="clinents-logos">
				<div class="client-img-container">
					<div class="client-img-fitter">
						<img src="../assets/img/client-logo-01.png" alt="" />
					</div>
					<div class="client-img-fitter">
						<img src="../assets/img/client-logo-02.png" alt="" />
					</div>
					<div class="client-img-fitter">
						<img src="../assets/img/client-logo-03.png" alt="" />
					</div>
					<div class="client-img-fitter">
						<img src="../assets/img/client-logo-04.png" alt="" />
					</div>
					<div class="client-img-fitter">
						<img src="../assets/img/client-logo-05.png" alt="" />
					</div>
					<div class="client-img-fitter">
						<img src="../assets/img/client-logo-06.png" alt="" />
					</div>
				</div>
			</div>
		</div>
	</header>
</template>

<script>
export default {
	name: "HeaderPage",
};
</script>

<style scoped lang="scss">
@import "../css/global.scss";

header {
	width: 100%;
}
// Top header SCSS section
.container-top {
	// border: 2px solid green;
	background-color: white;
	width: 100%;
	position: fixed;
	top: 0;
	left: 0;
	right: 0;
	z-index: 20px;
	display: flex;
	justify-content: center;
	box-shadow: 0 0.1px 15px rgb(197, 196, 196);

	.header-top {
		// border: 2px solid yellow;
		height: 75px;
		width: 1150px;
		display: flex;
		justify-content: space-between;

		.logo {
			height: 75px;
			width: 160px;
			display: flex;
			align-items: center;
		}

		.nav-section {
			// border: 2px solid black;
			height: 75px;
			width: 850px;
			display: flex;
			align-items: center;
			justify-content: space-between;

			nav {
				display: flex;
				gap: 1.6rem;

				a {
					color: #0b0b0b;
					display: flex;
					align-items: center;
					font-stretch: 2px;

					i {
						margin-left: 7px;
						font-size: 12px;
					}
				}
			}

			input {
				padding: 1rem 0.8rem;
				font-size: 1rem;
				border-radius: 3px;
				background-color: #f5f5f5;
				border: none;
			}
		}
	}
}

// Bottom header SCSS section
.container-bottom {
	// border: 2px solid black;
	margin: 0 auto;
	margin-top: 75px;
	height: 875px;
	width: 1365px;
	display: flex;
	flex-wrap: wrap;
	justify-content: center;

	.text-presentation-container {
		// border: 2px solid purple;
		height: 75%;
		width: 40%;
		display: flex;
		justify-content: center;
		align-items: center;

		.text-section {
			//   border: 5px solid purple;
			height: 20rem;
			margin-left: 5.4rem;
			display: flex;
			flex-direction: column;
			justify-content: space-evenly;

			.text-box {
				h1 {
					font-size: 2.5rem;
					color: #3f3a64;
					margin-bottom: 0.6rem;
				}

				p:nth-child(2) {
					color: #aeadae;
					font-weight: 500;
				}
			}

			.button-download {
				button {
					background-color: #20ad96;
					border: none;
					border-radius: 5px;
					padding: 1rem 3rem;
					color: white;
					font-weight: 800;
					transition: 0.2s ease-in-out;

					&:hover {
						background-color: #3f3a64;
						cursor: pointer;
					}

					i {
						margin-right: 1rem;
					}
				}
			}

			.free-sample {
				p:last-child {
					color: #aeadae;
					font-weight: 500;

					span {
						color: #20ad96;
						font-weight: 600;

						i {
							margin-left: 0.3rem;
						}
					}
				}
			}
		}
	}

	.big-pic-presentation {
		// border: 2px solid firebrick;
		height: 75%;
		width: 60%;
		display: flex;
		justify-content: center;
		align-items: center;

		.img-fitter {
			// border: 2px solid brown;
			height: 500px;
			width: 500px;
			border-radius: 50%;
			overflow: hidden;
		}
	}

	.clinents-logos {
		// border: 2px solid yellowgreen;
		height: 25%;
		width: 100%;
		display: flex;
		justify-content: center;

		.client-img-container {
			// border: 2px solid blue;
			width: 1200px;
			height: 218, 75px;
			display: flex;
			flex-wrap: wrap;

			.client-img-fitter {
				// border: 2px solid black;
				height: 100%;
				width: calc(100% / 6);
				opacity: 0.5;

				img {
					object-fit: contain;
					scale: 0.4;
					height: 100%;
				}
			}
		}
	}
}
</style>