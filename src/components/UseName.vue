<template>
    <span>{{ name }}</span>
  </template>
  
  
  <script setup>
  import { ref, reactive, computed } from "vue";
  
  defineProps({
    name: String,
  });
  </script>