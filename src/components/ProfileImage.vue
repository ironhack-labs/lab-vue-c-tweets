<script setup>
defineProps({
    userImage: String,
})
</script>

<template>
    <img :src="userImage" class="profile" :alt="userHandle" />
</template>

