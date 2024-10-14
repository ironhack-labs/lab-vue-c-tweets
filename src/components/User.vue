<template>
    <span class="user">
      <span class="name">{{ user.name }}</span>
      <span class="handle">@{{ user.handle }}</span>
    </span>
  </template>
  
  <script setup>
    defineProps({
      user: Object,
    });
  </script>
  
  <style scoped>
  .user .name {
    font-weight: bold;
    margin-bottom: 0.5em;
    margin-right: 0.3em;
  }
  .user .handle {
    color: #536471;
    margin-left: 3px;
    margin-right: 3px;
  }
  </style>
  