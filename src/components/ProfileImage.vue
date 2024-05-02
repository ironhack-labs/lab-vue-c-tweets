
<script setup>
import {defineProps} from 'vue'

// Aquí digo que la prop image es de tipo String
const props = defineProps({
    image: String
})
</script>
<!-- aqui literalmente hago el componente ver tweet col20 -->
<template>
    <img :src="image" class="profile" alt="profile"/>
</template>


<style scoped></style>
