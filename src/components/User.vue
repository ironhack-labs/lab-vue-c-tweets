<script setup>
const props = defineProps({
    userData: Object
})
const { name, handle } = props.userData;
</script>

<template>
    <span class="user">
        <span class="name">{{ name }}</span>
        <span class="handle">{{ handle }}</span>
    </span>
</template>