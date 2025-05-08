<script setup>
const props = defineProps({
    image: String,
})
</script>

<template>
    <img :scr="image" class="profile" alt="profile"/>
</template>