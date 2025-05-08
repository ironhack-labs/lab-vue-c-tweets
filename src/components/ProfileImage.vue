<script setup>
const props = defineProps({
  image: String,
});
</script>

<template>
  <section>
    <img :src="props.image" class="profile" alt="profile" />
  </section>
</template>

<style scoped></style>
