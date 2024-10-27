<script setup>
const props = defineProps({
    time: String,
});
</script>

<template>
    <span class="timestamp"> {{ props.time }}</span>
</template>

<style scoped>

</style>