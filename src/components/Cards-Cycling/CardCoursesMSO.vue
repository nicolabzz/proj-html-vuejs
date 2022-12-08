<template>
	<div class="card">
		<div class="card-pic">
			<img :src="imgPic" alt="#" />
		</div>
		<div class="card-text">
			<p>{{ cost }}</p>
			<h3>{{ title }}</h3>
			<span><i class="fa-solid fa-sheet-plastic"></i>{{ info1 }}</span>
			<span><i class="fa-regular fa-user"></i>{{ info2 }}</span>
		</div>
	</div>
</template>

<script>


export default {
	name: "CardCoursesMSO",
	props: {
		imgPic: String,
		cost: String,
		title: String,
		info1: String,
		info2: String,
	},
};
</script>

<style scoped lang="scss">
@import "../../css/global.scss";

.card {
	// border: 1px solid purple;
	height: 221px;
	display: flex;
	align-items: center;
	padding: 15px;
	transition: 0.2s ease-in-out;

	&:hover {
		cursor: pointer;
		background-color: white;
		border-radius: 5px;
	}

	.card-pic {
		// border: 1px solid orange;
		height: 180px;
		width: 180px;
		border-radius: 50%;
		overflow: hidden;

		img {
			object-fit: cover;
			width: 100%;
			height: 100%;
		}
	}

	.card-text {
		// border: 2px solid black;
		height: 100%;
		width: 70%;
		padding: 1rem 0 0.6rem 1rem;

		p {
			font-size: 1.5rem;
			font-weight: bold;
			color: #20ad96;
		}

		h3 {
			color: #3f3a64;
			margin: 1.5rem 0;
			transition: 0.2s ease-in-out;

			&:hover {
				color: #20ad96;
				cursor: pointer;
			}
		}

		span {
			color: #aeadae;

			i {
				margin-right: 0.5rem;
			}
		}

		span:last-child {
			padding-left: 2.5rem;
		}
	}
}
</style>