
<script setup>
  const props = defineProps({
      timestamp: {
        type: String,
        required: true
      },
  })
</script>

<template>
  <span class="timestamp">{{ timestamp }}</span>
</template>