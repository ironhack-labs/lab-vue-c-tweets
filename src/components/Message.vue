<script setup>
const props = defineProps(["msg"]);
</script>

<template>
    <p class="message">{{ props.msg }}</p>
</template>