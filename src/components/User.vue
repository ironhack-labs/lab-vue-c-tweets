<script setup>
// Define props
const { props } = defineProps(["userData"]);
</script>

<template>
	<span class="user">
		<span class="name">{{ userData.name }}</span>
		<span class="handle">{{ userData.handle }}</span>
	</span>
</template>
