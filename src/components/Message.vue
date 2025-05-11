<template>
  <p class="message">{{ message }}</p>
</template>

<script setup>
const props = defineProps({
  message: {
    type: String,
    required: true,
  },
});
</script>
