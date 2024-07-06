<script setup>
defineProps({
    userName: String,
    userHandle: String,
})
</script>

<template>
    <span class="user">
        <span class="name">{{ userName }} </span>
        <span class="handle">{{ userHandle }}</span>
    </span>
</template>
