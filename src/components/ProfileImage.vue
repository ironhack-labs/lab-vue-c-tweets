<script setup>
defineProps({
    image:Object
})
</script>

<template>
<img
       
       :src="image.image"
       class="profile"
       :alt="image.name"
     />
</template>

<style scoped>

</style>