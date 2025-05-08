<script setup>
defineProps({
    userData: {
        type: Object,
        
    },
})

</script>

<template>

    
<template>
  <span class="user">
    <span class="name">{{ userData.name }}</span>
    <span class="handle">@{{ userData.handle }}</span>
  </span>
</template>


</template>

<style scoped>
</style>