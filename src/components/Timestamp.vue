<script setup>
import { defineProps } from 'vue';

const props = defineProps({
    time: String
})

</script>


<template>
 <span class="timestamp">{{ time }}</span>
</template>
  

  
<style></style>