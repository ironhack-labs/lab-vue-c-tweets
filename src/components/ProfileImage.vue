<template>
  <img :src="image" class="profile" alt="profile image" />
</template>

<script setup>
defineProps({
  image: String
});
</script>