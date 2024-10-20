<script setup>
defineProps(
    {
        image: String
    }
);
</script>
<template>
    <img v-bind:src=image class="profile" alt="profile" />
</template>