<template>
  <p class="message">{{ message }}</p>
</template>

<script setup>
defineProps({
  message: String
});
</script>

<style scoped>
.message {
  margin: 0.5em 0;
}
</style>
