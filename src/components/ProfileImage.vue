<template>
    <img :src="image" class="profile" alt="profile" />
  </template>
  
  <script setup>
    // Define la prop 'image'
    defineProps({
      image: String
    });
  </script>
  
  