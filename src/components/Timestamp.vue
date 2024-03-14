<script setup>
const props = defineProps({
    timestamp: String
})

const timestamp= props.timestamp

</script>

<template>

    <span class="timestamp">{{ timestamp }}</span>

</template>
