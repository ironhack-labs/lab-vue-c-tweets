<script setup>

defineProps({
  name: {
    type: String,
    required: true,
  },
  handle: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <span class="name">{{name }}</span>
  <span class="handle">{{ handle}}</span>
</template>
