<script setup>
const props = defineProps(["img"]);
</script>

<template>
   <img :src="props.img" class="profile" alt="user">
</template>
