<template>
	<div>
		<slot></slot> is: {{value}}
	</div>
</template>

<script>
	export default {
		name: "valueView",
		props: ["value"],
	};
</script>

<style scoped>
	div {
		background-color: #fcf;
	}
</style>