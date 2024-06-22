<template>
  <span class="message"> {{ message }}</span>
</template>

<script setup>
defineProps({
  message: String,
});
</script>
