<template>
  <p class="message">{{ message }}</p>
</template>

<script setup>
defineProps({
    message: String
})
</script>

<style scoped>
.message {
    font-size: 16px;
    margin: 8px;
}
</style>
