<script setup>
import { ref, defineProps } from 'vue';
const props = defineProps({
  time: {
    type: String,
    default: "Nov 30, 2020",
  }
});
</script>

<template>
    <span class="timestamp">{{ props.time }}</span>
</template>