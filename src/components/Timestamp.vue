<template>
    <span class="timestamp">{{ time }}</span>
  </template>
  
  <script setup>
  const props = defineProps({
    time: String,
  });
  </script>
  
  <style scoped>
  .timestamp {
    color: #536471;
    font-size: 1.1rem;
  }
  .timestamp::before {
    content: "·";
    padding-right: 0.3em;
    font-size: 1.1rem;
    font-weight: 600;
  }
  </style>
  