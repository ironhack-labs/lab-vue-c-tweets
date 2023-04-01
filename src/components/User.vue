<template>
    <span class="user">
        <span class="name">
            {{ name }}</span>
        <span class="handle">@{{ handle }}</span>
    </span>
</template>

<script setup>

const props = defineProps(['name', 'handle', 'user'])
</script>