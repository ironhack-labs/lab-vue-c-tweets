<template>
    <p class="message">
        {{ message }}
    </p>
</template>

<script setup>
const props = defineProps(['message'])
</script>