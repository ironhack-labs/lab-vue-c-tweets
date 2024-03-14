<script setup>
    defineProps ({
        imageUrl: String,
    })
</script>

<template>
    <img :src="imageUrl" class="profile" alt="profile"/>
</template>

<style scoped>

</style>
