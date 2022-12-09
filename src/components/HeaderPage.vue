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
					<img src="img/dark-logo.png" alt="" />
				</div>

				<!-- Nav options -->
				<div class="nav-section">
					<!-- <nav>
						<a
							v-for="(link, i) in arrLinksNav"
							:key="i"
							href="!#"
							class="hover-underline-animation"
							>{{ link }}<i class="fa-solid fa-chevron-down"></i
						></a>
					</nav> -->
					<LinksNavHeader :navData="navData" />

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
							<span class="hover-underline-animation">
								Get Free Sample <i class="fa-solid fa-arrow-right-long"></i>
							</span>
						</p>
					</div>
				</div>
			</div>

			<!-- Big Pic -->
			<div class="big-pic-presentation">
				
				<div class="dit1">
					<img src="img/maxcoach-shape-08.png/" alt="" />
				</div>
				<div class="dit2">
					<img src="img/maxcoach-shape-08.png" alt="" />
				</div>
				<div class="dit3">
					<img src="img/rose-circle.png" alt="" />
				</div>
				<div class="dit4">
					<img src="img/maxcoach-shape-07-150x150.png" alt="" />
				</div>
				<div class="dit5">
					<img src="img/maxcoach-shape-02.png" alt="" />
				</div>
				<div class="img-fitter">
					<img
						src="img/about-me-profile-ohm4dxoearqbxny7q3bq1pzbdgofdx0tobbeqcvzd0.jpg"
						alt=""
					/>
				</div>
			</div>

			<!-- Clients Logos -->
			<div class="clinents-logos">
				<div class="client-img-container">
					<div class="client-img-fitter">
						<img id="client1" src="img/client-logo-01.png" alt="" />
					</div>
					<div class="client-img-fitter">
						<img id="client2" src="img/client-logo-02.png" alt="" />
					</div>
					<div class="client-img-fitter">
						<img id="client3" src="img/client-logo-03.png" alt="" />
					</div>
					<div class="client-img-fitter">
						<img id="client4" src="img/client-logo-04.png" alt="" />
					</div>
					<div class="client-img-fitter">
						<img id="client5" src="img/client-logo-05.png" alt="" />
					</div>
					<div class="client-img-fitter">
						<img id="client6" src="img/client-logo-06.png" alt="" />
					</div>
				</div>
			</div>
		</div>
	</header>
</template>

<script>
import LinksNavHeader from "@/components/Cards-Cycling/LinksNavHeader.vue";

export default {
	name: "HeaderPage",
	components: {
		LinksNavHeader,
	},
	data() {
		return {
			navData: {
				links: [
					{
						link: "Home",
					},
					{
						link: "Pages",
					},
					{
						link: "Courses",
					},
					{
						link: "Features",
					},
					{
						link: "Blog",
					},
					{
						link: "Shop",
					},
				],
			},
		};
	},
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
	// position: fixed;
	top: 0;
	left: 0;
	right: 0;
	// z-index: 20px;
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
			cursor: pointer;
		}

		.nav-section {
			// border: 2px solid black;
			height: 75px;
			width: 850px;
			display: flex;
			align-items: center;
			justify-content: space-between;

			.links-nav {
				// flex: 0 0 16.66666666666667%;
			}

			.account {
				transition: 0.2s ease-in-out;
				scale: (1);

				&:hover {
					scale: (1.11);
					color: #20ad96;
					cursor: pointer;
				}
			}

			.search-section {
				// border: 2px solid black;
				padding-right: 0.5rem;
				background-color: #f5f5f5;
				border-radius: 5px;

				i {
					cursor: pointer;

					&:hover {
						color: #20ad96;
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
					font-size: 3rem;
					color: #3f3a64;
					margin-bottom: 0.6rem;
				}

				p:nth-child(2) {
					color: #8c89a2;
					font-weight: 500;
					line-height: 2rem;
					margin-bottom: 1rem;
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
					margin-bottom: 1.5rem;

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
					cursor: pointer;

					span {
						color: #20ad96;
						font-weight: 600;
						border-bottom: 0.1px solid rgb(236, 236, 236);
						position: relative;
						display: inline-block;

						&::after {
							content: "";
							position: absolute;
							width: 100%;
							height: 1px;
							bottom: 0;
							left: 0;
							background-color: rgb(236, 236, 236);
							transform-origin: bottom right;
							transition: transform 0.25s ease-out;
							color: #20ad96;
							z-index: 0;
						}

						&:hover::after {
							transform-origin: bottom left;
						}

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
		position: relative;

		.dit1 {
			position: absolute;
			left: 0;
		}
		.dit2 {
			position: absolute;
			left: 0;
			bottom: 19%;
		}
		.dit3 {
			position: absolute;
			left: 0;
			top: 0;
		}
		.dit4 {
			position: absolute;
			bottom: 3rem;
			right: 8rem;
			
		}
		.dit5 {
			position: absolute;
			right: 0;
			top: 8rem;
		}

		.img-fitter {
			// border: 2px solid brown;
			height: 550px;
			width: 550px;
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
					height: 100%;
				}

				#client1 {
					padding: 2.6rem;
				}

				#client2 {
					padding: 3.5rem;
				}

				#client3 {
					padding: 1.1rem;
				}

				#client4,
				#client5,
				#client6 {
					padding: 2rem;
				}
			}
		}
	}
}

.container-top {
	position: fixed;
	z-index: 20;
}
</style>