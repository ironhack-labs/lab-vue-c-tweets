<template>
  <img class="profile" :src="image" alt="profile picture" />
</template>

<script setup>
defineProps({
  image: String
});
</script>

<style scoped>
.profile {
  border-radius: 50%;
  height: 50px;
}
</style>
