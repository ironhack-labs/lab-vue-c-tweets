<script setup>
const props = defineProps({
    image: String, 
});
</script>

<template>
    <img :src="props.image" class="profile" alt="Profile Image"/>
</template>

<style scoped>
</style>