<script setup>
import { defineProps } from "vue";

defineProps({
  message: String,
});
</script>
<template>
  <p class="message">{{ message }}</p>
</template> 
