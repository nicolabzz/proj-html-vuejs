<template>
	<div class="links-section">
		<div class="address">
			<h3>{{ footerData.addressCol.linkTitle }}</h3>
			<p>{{ footerData.addressCol.location }}</p>
			<p>{{ footerData.addressCol.phone }}</p>
			<p>{{ footerData.addressCol.eMail }}</p>
		</div>

		<div class="social">
			<a
				href=""
				v-for="social in footerData.addressCol.social"
				:key="social.socialLink"
				:icon="`${social.socialLink}`"
			>
			</a>

			<!-- <a href=""><i class="fa-brands fa-square-facebook"></i></a>
			<a href=""><i class="fa-brands fa-twitter"></i></a>
			<a href=""><i class="fa-brands fa-instagram"></i></a>
			<a href=""><i class="fa-brands fa-linkedin"></i></a> -->
		</div>
	</div>
</template>

<script>
export default {
	name: "AddressLinksFooter",
	props: {
		footerData: Object,
	},
};
</script>

<style scoped lang="scss">
@import "../../css/global.scss";

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
			transition: 0.15s ease-in-out;
			cursor: pointer;
		}

		p:nth-child(4):hover {
			color: #20ad96;
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
			transition: 0.15s ease-in-out;

			&:hover {
				color: #20ad96;
			}
		}
	}
}
</style>