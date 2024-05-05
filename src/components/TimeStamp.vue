<script setup>
import { defineProps } from "vue";
const props = defineProps({
  timestamp: String,
});
//console.log(props.timestamp)
</script>

<template>
  <span class="timestamp">{{ timestamp }}</span>
</template>

<style scoped></style>
