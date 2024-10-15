<template>
    <span class="user">
      <span class="name">{{ userData.name }}</span>
      <span class="handle">@{{ userData.handle }}</span>
    </span>
  </template>
  
  <script setup>
  const props = defineProps({
    userData: Object,
  });
  </script>
  
  <style scoped>
  .name {
    font-weight: bold;
    margin-bottom: 0.5em;
    margin-right: 0.3em;
  }
  .handle {
    color: #536471;
  }
  </style>
  