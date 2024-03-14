<script setup>
defineProps({
    message: String
})
</script>

<template>
    <p>{{ message }}</p>
</template>

<style scoped>
    p {
        white-space: pre-line;
        text-align: justify;
    }
</style>