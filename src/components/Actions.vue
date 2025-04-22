<template>
    <div class="actions">
      <i class="far fa-comment" data-type="comment" @click="handleAction"></i>
      <i class="fas fa-retweet" data-type="retweet" @click="handleAction"></i>
      <i class="far fa-heart" data-type="like" @click="handleAction"></i>
      <i class="fas fa-share" data-type="share" @click="handleAction"></i>
    </div>
  </template>
  
  <script setup>
  import { defineEmits } from 'vue';
  
  const emit = defineEmits();
  
  const handleAction = (event) => {
    const target = event.target;
    if (target.tagName === 'I') {
      const actionType = target.getAttribute('data-type');
      emit('action', actionType); // Emitir el tipo de acción
    }
  };
  </script>
  
  <style scoped>
  .actions {
    padding: 5px 5px;
    width: 360px;
    display: flex;
    justify-content: space-between;
    color: #536471;
  }
  </style>
  