<template>
    <p class="message">{{ content }}</p>
  </template>
  
  <script setup>
  import { defineProps } from 'vue';
  
  const props = defineProps({
    content: {
      type: String,
      required: true
    }
  });
  </script>
  
  <style scoped>
  .message {
    text-align: left;
    font-stretch: 100%;
    font-weight: 400;
    line-height: 1.6rem;
    overflow-wrap: break-word;
    white-space: pre-wrap;
  }
  </style>
  