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

		<div>
			<h1>Getting props or data from slot and handle On Parent Component</h1>
			<base-layout></base-layout>
		</div>
	</div>
	<!-- eslint-disable -->
</template>
<script>
import HeaderComponet from "./HeaderComponet.vue";
import BodyComponent from "./BodyComponent.vue";
import FooterComponent from "./FooterComponent.vue";
import BaseLayout from "./SoltProps/BaseLayout.vue";
export default {
	components: {
		"header-component": HeaderComponet,
		"body-component": BodyComponent,
		"footer-component": FooterComponent,
		"base-layout": BaseLayout,
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