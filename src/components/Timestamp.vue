<template>
  <section>
    <span class="timestamp">{{ props.time }}</span>
  </section>
</template>

<script setup>
const props = defineProps({
  time: String,
});
</script>

<style scoped></style>
