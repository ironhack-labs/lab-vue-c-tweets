<template>
  <span class="user">
    <span class="name">{{ name }}</span>
    <span class="handle"> {{ handle }}</span>
  </span>
</template>

<script setup>
import { defineProps } from "vue";

const props = defineProps({
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
