<script setup>

import { defineProps } from 'vue';

defineProps({
  img: String,
})

</script>
<template>
  <img :src="img" class="profile" alt="profile" />
</template> 