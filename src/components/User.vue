<template>
    <div class="user">
      <span class="username">{{ username }}</span>
      <span class="handle">{{ handle }}</span>
    </div>
  </template>
  
  <script setup>
  import { defineProps } from 'vue';
  
  const props = defineProps({
    username: {
      type: String,
      required: true
    },
    handle: {
      type: String,
      required: true
    }
  });
  </script>
  
  <style scoped>
  .user {
    display: flex;
    flex-direction: column;
  }
  .username {
    font-weight: bold;
  }
  .handle {
    color: gray;
  }
  </style>
  