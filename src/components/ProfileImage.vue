<!-- src/components/ProfileImage.vue -->
<template>
    <img :src="src" alt="Profile picture" class="profile" />
  </template>
  
  <script setup>
  defineProps({
    src: {
      type: String,
      required: true
    }
  })
  </script>
  
  <style scoped>

  </style>