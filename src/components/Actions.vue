<script setup>
defineProps({
    image: String
})
</script>

<template>
    <img :src="image" class="profile" alt="profile image" />

</template>

<style scoped>
.profile {
  width: 48px;
  height: 48px;
  border-radius: 50%;
  object-fit: cover;
}
</style>