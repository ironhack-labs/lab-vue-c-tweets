<script setup>
import { ref, defineProps } from 'vue';
const props = defineProps({
  userData: {
    type: Object,
    default: () => ({
      name: "Ironhack",
      image: "https://i.imgur.com/9yw1Fyw.jpg",
      handle: "ironhack",
    }),
  }
});
</script>

<template>
<span class="user">
    <span class="name">{{ props.userData.name }}</span>
    <span class="handle">@{{ props.userData.handle }}</span>
</span>
</template>