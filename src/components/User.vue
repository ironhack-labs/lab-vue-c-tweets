<script setup>
const props = defineProps({
    user: Object
})
const { name, handle } = props.user;
</script>

<template>
    <span class="user">
        <span class="name">{{ name }}</span>
        <span class="handle">{{ handle }}</span>
    </span>
</template>