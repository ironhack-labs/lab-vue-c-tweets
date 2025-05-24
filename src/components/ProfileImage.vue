<template>
  <section>
    <img :src="props.image" class="profile" alt="profile" />
  </section>
</template>

<script setup>
const props = defineProps({
  image: String,
});
</script>

<style scoped></style>
