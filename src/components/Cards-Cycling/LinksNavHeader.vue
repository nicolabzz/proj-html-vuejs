<template>
	<nav>
		<a
			v-for="obj in navData.links"
			:key="obj.link"
			class="hover-underline-animation"
		>
			<span>{{ obj.link }}</span>
			<i class="fa-solid fa-chevron-down"> </i>
		</a>
	</nav>
</template>

<script>
export default {
	name: "LinksNavHeader",
	props: {
		navData: Object,
	},
};
</script>

<style lang="scss" scoped>
@import "../../css/global.scss";

nav {
	display: flex;
	gap: 1.6rem;

	a {
		color: #0b0b0b;
		display: flex;
		align-items: center;
		font-stretch: 2px;
		position: relative;
		cursor: pointer;

		i {
			margin-left: 7px;
			font-size: 12px;
		}

		&:hover {
			color: #20ad96;
		}
	}

	.hover-underline-animation {
		position: relative;
		text-decoration: none;
	}

	.hover-underline-animation::after {
		content: "";
		position: absolute;
		width: 100%;
		transform: scaleX(0);
		height: 2px;
		bottom: 0;
		left: 0;
		background-color: #20ad96;
		transform-origin: bottom right;
		transition: transform 0.25s ease-out;
	}

	.hover-underline-animation:hover::after {
		transform: scaleX(1);
		transform-origin: bottom left;
	}
}
</style>