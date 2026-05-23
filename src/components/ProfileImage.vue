<script setup>
import { ref, defineProps } from 'vue';

const props = defineProps({
    image: {
        type: String,
        default: "https://i.imgur.com/9yw1Fyw.jpg"
    }
});
</script>

<template>
    <img
      :src="props.image"
      class="profile"
      alt="profile"
    />
</template>