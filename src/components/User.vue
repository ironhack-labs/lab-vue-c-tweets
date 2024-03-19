<script setup>
defineProps	({
    username: String,
    handle: String
})
</script>

<template>
<span class="name">{{ username }}</span>
<span class="handle">@{{ handle }}</span>
</template>