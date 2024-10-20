<script setup>
let props = defineProps(
    {
        message: String
    }
)
</script>
<template>
    <p class="message">{{ props.message }}</p>
</template>