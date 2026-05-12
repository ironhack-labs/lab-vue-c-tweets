<template>
  <img :src="image" class="profile" :alt="alt" />
</template>

<script setup>
  defineProps(['image', 'alt']);
</script>