<script setup>
import { defineProps } from 'vue'

// Definimos los props que vamos a recibir.
// Fíjate que aquí pone "movies", por lo tanto, cuando pasemos por prop en App.vue los datos deberemos referenciarlos como "movies".
const props = defineProps({
  user: {
    type: Object,
    required: true,
  }
})
</script>

<template>
  <span class="user">
    <span class="name">{{user.name}}</span>
    <span class="handle">{{user.handle}}</span>
  </span>
</template>

<style scoped>

</style>