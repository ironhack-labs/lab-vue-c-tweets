<script setup>
const props = defineProps({
  message: String,
});
</script>

<template>
  <div>
    <p class="message">
      {{ props.message }}
    </p>
  </div>
</template>

<style scoped></style>
