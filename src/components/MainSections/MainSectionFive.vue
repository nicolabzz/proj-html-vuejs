<template>
	<!-- Fifth section -->
	<main>
		<div class="container">
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
							Courses fom Expert' s Perspective</a
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

				<CardBlogMS5 
				v-for="objCard in arrBlogCards"
				:key="objCard.id"
				:img-pic="objCard.imgSrc"
				:work="objCard.workType"
				:description="objCard.text"
				:date="objCard.creationDate"
				:viewed="objCard.views"
				/>

			<div class="card-blog"></div>
		</div>
	</main>
</template>

<script>
import CardBlogMS5 from "../Cards-Cycling/CardBlogMS5.vue";
export default {
	name: "MainSectionFive",
	components: {
		CardBlogMS5,
	},
	data() {
		return {
			arrBlogCards: [
				{
					imgSrc: "img/artist-blog-03-480x352.jpeg",
					workType: "ARTIST",
					text: "Brush Strokes Energize Tree in Paintings",
					creationDate: " May 15, 2020",
					views: "688 views",
				},
				{
					imgSrc: "img/artist-blog-01-480x352.jpg",
					workType: "ARTIST",
					text: "Pocket-Sized Notebooks Hold Miniature Paintings",
					creationDate: " May 15, 2020",
					views: "603 views",
				},
			],
		};
	},
};
</script>

<style scoped lang="scss">
@import "../../css/global.scss";

main {
	background-color: #f5f1ed;
	height: 650px;
	display: flex;
	align-items: center;
}

.container {
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
				transition: 0.15s ease-in;
				display: flex;
				color: #3f3a64;

				&:hover {
					color: #20ad96;
				}

				i {
					margin-right: 1rem;
				}
			}
		}
	}
}
</style>