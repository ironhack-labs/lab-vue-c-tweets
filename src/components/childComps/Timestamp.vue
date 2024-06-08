<!-- HTML -->
<template>
  <span class="timestamp">{{ tweetChildTimestamp }}</span>
</template>

<!-- JS  -->
<script setup>
import { ref, reactive, computed } from "vue";

defineProps({
  tweetChildTimestamp: String,
});
</script>
