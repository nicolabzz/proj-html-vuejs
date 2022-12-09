<template>
	<div class="card-blog">
		<div class="pic">
			<img :src="imgPic" alt="" />
		</div>
		<div class="text">
			<h4>{{ work }}</h4>
			<h3>{{ description }}</h3>
			<span><i class="fa-regular fa-calendar"></i>{{ date }}</span>
			<span><i class="fa-regular fa-eye"></i>{{ viewed }}</span>
		</div>
	</div>
</template>

<script>
export default {
	name: "CardBlogMS5",
	props: {
		imgPic: String,
		work: String,
		description: String,
		date: String,
		viewed: String,
	},
};
</script>

<style scoped lang="scss">
@import "../../css/global.scss";
.card-blog {
	// border: 2px solid firebrick;
	padding: 1rem;
	.pic {
		// border: 3px solid blue;
		width: 100%;
		border-top-left-radius: 5px;
		border-top-right-radius: 5px;
		height: 55%;
		overflow: hidden;

		img {
			transition: 1.3s ease-in-out;
      cursor: pointer;

			&:hover {
				scale: 1.1;
			}
		}
	}

	.text {
		// border: 2px solid green;
		width: 100%;
		height: 45%;
		padding: 1.7rem 0 0 1rem;
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
			margin-bottom: 1rem;
			padding: 5px 0 0 0;
      transition: .2s ease-in-out;
      cursor: pointer;

			&:hover {
				color: #20ad96;
			}
		}

		span {
			color: #7e7e7e;
			font-weight: 600;
			font-size: 0.9rem;
      cursor: pointer;
      

			i {
				margin-right: 0.5rem;
			}
		}

		span:last-child {
			margin-left: 1.4rem;
		}
	}
}
</style>