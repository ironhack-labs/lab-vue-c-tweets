<template>
    <span class="timestamp">{{ time }}</span>
</template>
<script setup>
import { ref } from 'vue';
const props = defineProps({
    time: {
        type: String,
        required: true
    }
});
</script>