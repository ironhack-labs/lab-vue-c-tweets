<script setup>
const props = defineProps({
  time: String,
});
</script>

<template>
  <section>
    <span class="timestamp">{{ props.time }}</span>
  </section>
</template>

<style scoped></style>
