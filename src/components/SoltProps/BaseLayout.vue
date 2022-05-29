<template>
	<div>
		<list>
			<template v-slot:propSlot="info">
				<h1>Id: {{ info.item.id }}</h1>
				<h2>Name: {{ info.item.name }}</h2>
				<h3>Last {{ info.item.last }}</h3>
			</template>
		</list>
	</div>
</template>

<script>
import DynamicList from "./DynamicList.vue";
export default {
	components: {
		list: DynamicList,
	},
};
</script>
