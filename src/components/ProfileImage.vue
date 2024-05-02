<script setup>
import { defineProps } from "vue";

const props = defineProps({
  image: String,
});
console.log(props.image);
</script>

<template>
  <section>
    <img :src="image" class="profile" alt="profile" />
  </section>
</template>


