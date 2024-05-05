<script setup>
import { defineProps } from "vue";

const props = defineProps({
  message: String,
});
//console.log(props.message)
</script>

<template>
  <p class="message">{{ message }}</p>
</template>

<style scoped></style>
