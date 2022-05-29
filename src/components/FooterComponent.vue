/* eslint-disable */
<template>
	<div>
		<slot name="footer"> </slot>
		<div>
			<h2>Adding content to footer</h2>
		</div>
	</div>
</template>
<script>
export default {
	mounted() {
		// We can see if the named slot bring info access
		console.log(this.$slots.footer);
	},
};
</script>
<style scoped></style>