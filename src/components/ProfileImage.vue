<script setup>
    defineProps({
        image: {
            type: String,
        },
    });
</script>
<template>
    <img :src="image" alt="profile" class="profile" /> 
</template>