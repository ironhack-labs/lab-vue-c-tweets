<script setup>

const props = defineProps({
    imageSrc: String
});

</script>

<template>
    <img :src="imageSrc" class="profile" alt="profile" />
</template>

<style scoped></style>