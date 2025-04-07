<script setup>
import { defineProps} from "vue";

defineProps({
  timestamp: String,
  handle: String,
});
</script>

<template>
  <span class="user">
    <span class="timestamp">{{ timestamp }}</span>
  </span>
</template>
