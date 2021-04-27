<template>
	<div>
		<label>Enter value:
			Enter value: <input type="text" :value="value" @input="$emit('input', $event.target.value)"/>
		</label>
	</div>
</template>

<script>
	export default {
		name: 'DateStringSelector',
		props: ['value'],
		emits: ['input'],
	};
</script>

<style scoped>
	div {
		background-color: #cff;
	}

	label {
		color: red;
	}
</style>