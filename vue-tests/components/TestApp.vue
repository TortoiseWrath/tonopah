<template>
	<h1>It's vue.</h1>
	<div>
		<router-link to="/other">Another view</router-link>
	</div>
	<value-form v-model="value"></value-form>
	<value-view :value="value">My value</value-view>
</template>

<script>
	import valueView from "./valueView.vue";
	import valueForm from "./valueForm.vue";

	export default {
		name: 'TestApp',
		data() {
			return {
				value: 'default',
			}
		},
		components: {
			valueForm,
			valueView,
		},
		created() {
			console.log('app created');
		},
	};
</script>

<style scoped>
	div {
		font-family: 'Comic Sans MS', fantasy;
	}
</style>