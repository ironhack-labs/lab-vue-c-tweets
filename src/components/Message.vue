<template>
    <p class="message">
        {{ sms }}
    </p>
</template>
<script setup>
import { ref } from 'vue';
const props = defineProps({
    sms: {
        type: String,
        required: true
    }
});
</script>