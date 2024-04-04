
<script setup>
  const props = defineProps({
      image: {
        type: String,
        required: true
      },
  })
</script>

<template>
  <img
    :src="image"
    class="profile"
    alt="profile"
  />
</template>