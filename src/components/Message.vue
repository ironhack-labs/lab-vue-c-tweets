<!-- src/components/Message.vue -->
<template>
    <div class="message">
      {{ content }}
    </div>
  </template>
  
  <script setup>
  defineProps({
    content: {
      type: String,
      required: true
    }
  })
  </script>
  
  <style scoped>

  </style>
  