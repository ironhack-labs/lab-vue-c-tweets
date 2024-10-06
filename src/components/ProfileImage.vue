
<script setup>
  import { defineProps } from 'vue';
  
  const props = defineProps({
    image: {
      type: String,
      required: true,
    },
    name: {
      type: String,
      required: true,
    },
  });
  </script>

<template>
    <img :src="image" class="profile" :alt="`${name} profile`" />
  </template>
  
  <style scoped>
  </style>
  