/* eslint-disable */
<template>
	<!-- eslint-disable -->
	<div>
		<header-component>
			<template v-slot:header>
				<!-- #hedaer short name on template -->
				<h1>{{ headerMsg }}</h1>
			</template>
		</header-component>

		<body-component>
			<template v-slot:body>
				<h1>{{ bodyMsg }}</h1>
			</template>
		</body-component>

		<footer-component>
			<template v-slot:footer>
				<h1>{{ footerMsg }}</h1>
			</template>
		</footer-component>
	</div>
	<!-- eslint-disable -->
</template>
<script>
import HeaderComponet from "./HeaderComponet.vue";
import BodyComponent from "./BodyComponent.vue";
import FooterComponent from "./FooterComponent.vue";
export default {
	components: {
		"header-component": HeaderComponet,
		"body-component": BodyComponent,
		"footer-component": FooterComponent,
	},
	data() {
		return {
			headerMsg: "Im the header component",
			bodyMsg: "Im the body componet",
			footerMsg: "Im the footer component",
		};
	},
};
</script>
<style scpoed>
/* eslint-disable */
</style>