<script setup>
import { ref, defineProps } from 'vue';

const props = defineProps({
  message: {
    type: String,
    default: "On December 7th, we will be hosting a #webinar that will introduce you to #SQL! Are you ready? 🚀"
    }
});
</script>

<template>
    <p class="message">{{ props.message }}</p>
</template>