<template>
	<!-- Fifth section -->
	<main>
		<section class="blogs-card-container">
			<div class="card-text">
				<h4>ENJOYABLE INSIGHT</h4>
				<h1>Most Viwed <span>Best Blogs</span></h1>
				<ul>
					<li>
						<a href=""
							><i class="fa-solid fa-arrow-right-long"></i> Become a Better
							Blogger: Content Planning</a
						>
					</li>
					<li>
						<a href=""
							><i class="fa-solid fa-arrow-right-long"></i> Promoting Your
							Online Buisness on Printset</a
						>
					</li>
					<li>
						<a href=""
							><i class="fa-solid fa-arrow-right-long"></i> Gamification and
							Game-Based Learning</a
						>
					</li>
					<li>
						<a href=""
							><i class="fa-solid fa-arrow-right-long"></i> Designing an Online
							Courses fom Expert's Perspective</a
						>
					</li>
					<li>
						<a href=""
							><i class="fa-solid fa-arrow-right-long"></i> Why Online Courses
							Are the Future of Education</a
						>
					</li>
				</ul>
			</div>

			<div class="card-blog">
				<div class="card-pic">
					<img src="../assets/img/artist-blog-03-480x352.jpeg" alt="" />
				</div>
				<div class="card-blog-text">
					<h4>ARTIST</h4>
					<h3>Brush Strokes Energize Tree in Paintings</h3>
					<span><i class="fa-regular fa-calendar"></i> May 15, 2020</span>
					<span><i class="fa-regular fa-eye"></i> 688 views</span>
				</div>
			</div>

			<div class="card-blog"></div>
		</section>
	</main>
</template>

<script>
export default {
	name: "MainSectionFive",
};
</script>

<style scoped lang="scss">
@import "../css/global.scss";

main {
	background-color: #f5f1ed;
	height: 650px;
	display: flex;
	align-items: center;
}

.blogs-card-container {
	// border: 2px solid cadetblue;
	width: 1150px;
	height: 450px;
	margin: auto;
	padding: 0 1rem;
	display: flex;
	flex-wrap: wrap;

	div[class*="card"] {
		// border: 2px solid firebrick;
		width: calc(100% / 3);
	}

	.card-text {
		display: flex;
		flex-direction: column;
		gap: 1rem;
		padding: 2rem 0;

		h4 {
			color: #9ea4a5;
			font-weight: 600;
			letter-spacing: 2px;
		}

		h1 {
			color: #3f3a64;
			font-size: 2rem;
			margin-bottom: 1.5rem;

			span {
				color: #20ad96;
				font-weight: 500;
			}
		}

		li {
			list-style-type: none;
			padding-bottom: 1.5rem;

			a {
				font-weight: 900;
				font-size: 0.8rem;
				display: block;

				i {
					margin-right: 1rem;
				}
			}
		}
	}

	.card-blog {
		padding: 0 1rem;
		// border: 2px solid firebrick;

		.card-pic {
			// border: 3px solid blue;
			width: 100%;
			border-top-left-radius: 5px;
			border-top-right-radius: 5px;
			height: 55%;
			overflow: hidden;
		}

		.card-blog-text {
			// border: 2px solid green;
			width: 100%;
			height: 40%;
			padding: 1rem 0 0 1rem;
			background-color: white;
			border-bottom-left-radius: 5px;
			border-bottom-right-radius: 5px;

			h4 {
				color: #9ea4a5;
				letter-spacing: 2px;
				font-weight: 500;
			}

			h3 {
				color: #3f3a64;
				font-weight: 800;
				line-height: 2rem;
				margin-bottom: 1.5rem;
			}

			span {
				color: #7e7e7e;
				font-weight: 600;
				font-size: 0.9rem;

				i {
					margin-right: 0.5rem;
				}
			}

			span:last-child {
				margin-left: 1.4rem;
			}
		}
	}
}
</style>