<template>
    <img :src="user.image" class="profile" alt="profile" />
</template>

<script setup>
const props = defineProps({
    image: String
})
</script>
