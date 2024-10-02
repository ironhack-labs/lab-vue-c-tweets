<script setup>
import { ref } from 'vue';
const realHTML = ref(`
  <i class='far fa-comment'></i>
  <i class='fas fa-retweet'></i>
  <i class='far fa-heart'></i>
  <i class='fas fa-share'></i>
`);

</script>

<template>
    <div v-html="realHTML"></div>
</template>

<style scoped>

</style>