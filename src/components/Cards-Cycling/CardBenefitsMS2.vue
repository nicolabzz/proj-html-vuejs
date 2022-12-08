<template>
	<div class="card">
		<div class="card-pic">
			<img :src="imgPic" alt="" />
		</div>
		<div class="card-text">
			<h2>{{ title }}</h2>
			<p>
				{{ content }}
			</p>
			<a
				class="hover-underline-animation"
				href="https://www.youtube.com/watch?v=dQw4w9WgXcQ"
				>{{ link }} <i class="fa-solid fa-arrow-right-long"></i
			></a>
		</div>
	</div>
</template>

<script>
export default {
	name: "CardBenefitsMS2",
	props: {
		imgPic: String,
		title: String,
		content: String,
		link: String,
	},
};
</script>

<style scoped lang="scss">
@import "../../css/global.scss";

.card {
	// border: 2px solid greenyellow;
	width: calc(100% / 3);

	.card-pic {
		// border: 2px solid salmon;
		height: 50%;
		width: 100%;
		padding: 0.7rem 0 0 50px;

		img {
			height: 90%;
			object-fit: contain;
			object-position: left;
		}
	}

	.card-text {
		// border: 1px solid black;
		height: 50%;
		padding: 0.5px 0 0 45px;

		h2 {
			color: #3f3a64;
		}

		p {
			color: #696969;
			padding: 2rem 0;
		}

		a {
			color: #8c89a2;
			font-weight: 800;
			font-size: 13px;
			position: relative;

			&:hover {
				color: #20ad96;
			}

			&::before {
				content: "";
				position: absolute;
				display: block;
				width: 100%;
				height: 0.1px;
				bottom: -5px;
				left: 0;
				background-color: #8c89a2;
				transform: scaleX(0);
				transform-origin: top left;
				transition: transform 0.4s ease-in-out;
			}

			&:hover::before {
				transform: scaleX(1);
			}
		}
	}
}
</style>