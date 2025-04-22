<template>
    <img :src="image" alt="Profile Image" class="profile" />
  </template>
  
  <script setup>
  import { defineProps } from 'vue';
  
  const props = defineProps({
    image: {
      type: String,
      required: true
    }
  });
  </script>
  
  <style scoped>
  .profile {
    width: 50px;
    height: 50px;
    border-radius: 50px;
    margin-right: 10px;
  }
  </style>
  