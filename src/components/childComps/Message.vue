<!-- HTML -->
<template>
  <p class="message">
    {{ tweetChildMessage }}
  </p>
</template>

<!-- JS  -->
<script setup>
import { ref, reactive, computed } from "vue";

defineProps({
  tweetChildMessage: String,
});
</script>
