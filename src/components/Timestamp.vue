<script>

const props = defineProps({
  user: {
  name: String,
  img: String,
  handle: String,
  },  
  timestamp: String, 
  message: String,
});

</script>

<template>
    <span class="timestamp">{{timestamp}}</span>
</template>