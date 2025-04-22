<template>
    <span class="timestamp">{{ time }}</span>
  </template>
  
  <script setup>
  import { defineProps } from 'vue';
  
  const props = defineProps({
    time: {
      type: String,
      required: true
    }
  });
  </script>
  
  <style scoped>
  .timestamp {
    color: gray;
    font-size: 0.85em;
  }
  </style>
  