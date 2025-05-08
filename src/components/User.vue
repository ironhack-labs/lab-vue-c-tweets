<!-- src/components/UserComponent.vue -->
<template>
    <div class="user-info">
      <span class="name">{{ name }}</span>
      <span class="handle">@{{ handle }}</span>
      <Timestamp :timestamp="timestamp" />
    </div>
  </template>
  
  <script setup>
  import Timestamp from './Timestamp.vue'
  
  defineProps({
    name: {
      type: String,
      required: true
    },
    handle: {
      type: String,
      required: true
    },
    timestamp: {
      type: String,
      required: true
    }
  })
  </script>
  
  <style scoped>

  </style>
  