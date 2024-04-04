
<script setup>
  const props = defineProps({
      message: {
        type: String,
        required: true
      },
  })
</script>

<template>
  <p class="message">
    {{ message }}
  </p>
</template>