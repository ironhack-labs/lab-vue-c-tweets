
<script setup>
  const props = defineProps({
      name: {
        type: String,
        required: true
      },
      handle: {
        type: String,
        required: true
      }
  })
</script>

<template>
  <span class="user">
    <span class="name">{{ name }}</span>
    <span class="handle">@{{ handle }}</span>
  </span>
</template>