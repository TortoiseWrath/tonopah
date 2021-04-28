<template>
	<div>
		<label>Enter value:
			<input type="text" :value="modelValue" @input="$emit('update:modelValue', $event.target.value)"/>
		</label>
	</div>
</template>

<script>
	export default {
		name: 'valueForm',
		props: ['modelValue'],
		emits: ['update:modelValue'],
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