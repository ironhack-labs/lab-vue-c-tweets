<!-- HTML -->
<template>
  <p class="message">
    {{ message }}
  </p>
</template>

<!-- JS  -->
<script setup>
defineProps({
  message: String,
});
</script>
