<script setup>
const props = defineProps(["time"]);
</script>

<template>
    <span class="timestamp">{{ props.time }}</span>
</template>