<script setup>
import { defineProps } from 'vue'

// Definimos los props que vamos a recibir.
// Fíjate que aquí pone "movies", por lo tanto, cuando pasemos por prop en App.vue los datos deberemos referenciarlos como "movies".
const props = defineProps({
  timestamp: {
    type: String,
    required: true,
  }
})
</script>

<template>
    <span class="timestamp">{{timestamp}}</span>
</template>

<style scoped>

</style>