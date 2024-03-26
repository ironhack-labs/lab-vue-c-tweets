<script setup>

const props = defineProps({
    image: { type: String },
})

</script>

<template>
    <img :src="props.image" class="profile" alt="profile" />
</template>

<style scoped>
  .profile {
    width: 50px;
    height: 50px;
    border-radius: 50px;
    margin-right: 10px;
  }
</style>