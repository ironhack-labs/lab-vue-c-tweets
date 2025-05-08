<script setup>
const props = defineProps({
  user: {
    name: String,
    image: String,
    handle: String,
  },
});
</script>

<template>
  <section>
    <span class="user">
      <span class="name">{{ props.user.name }}</span>
      <span class="handle">{{ props.user.handle }}</span>
    </span>
  </section>
</template>

<style scoped></style>
