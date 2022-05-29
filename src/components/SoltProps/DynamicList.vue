<template>
	<div>
		<div v-for="item in list" :key="item.id">
			<slot name="propSlot" :item="item"></slot>
		</div>
	</div>
</template>
<script>
export default {
	data() {
		return {
			list: [
				{
					id: 0,
					name: "Marcos",
					last: "Torres",
				},
				{
					id: 1,
					name: "Juan",
					last: "Aguirre",
				},
			],
		};
	},
};
</script>
