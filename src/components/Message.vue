<script setup>
defineProps({
    message:String
})

</script>

<template>

<p class="message">
        <!-- On December 7th, we will be hosting a #webinar that will introduce you
        to #SQL! Are you ready? 🚀 -->
        {{ message }}
      </p>
</template>

<style scoped>

</style>