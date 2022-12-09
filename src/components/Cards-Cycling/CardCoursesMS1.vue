<template>
	<div class="card-container">
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
	</div>
</template>

<script>
export default {
	name: "CardCoursesMS1",
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

.card-container {
	// border: 1px solid greenyellow;
	display: flex;
	align-items: center;
	justify-content: center;

	.card {
		// border: 1px solid purple;
		height: 221px;
		width: 95%;
		display: flex;
		align-items: center;
		justify-content: space-between;
		padding: 15px;
		transition: 0.2s ease-in-out;

		&:hover {
			background-color: white;
			border-radius: 5px;
			box-shadow: 1px 1px 50px rgb(218, 218, 218);
		}

		.card-pic {
			// border: 1px solid orange;
			height: 170px;
			width: 170px;
			border-radius: 50%;
			overflow: hidden;

			&:hover {
				cursor: pointer;
			}

			img {
				object-fit: cover;
				width: 100%;
				height: 100%;
			}
		}

		.card-text {
			// border: 2px solid black;
			height: 100%;
			width: 65%;
			padding: 1rem 0 0rem 1rem;

			p {
				font-size: 1.5rem;
				font-weight: 900;
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
}
</style>