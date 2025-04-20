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
    <span class="user">
        <span class="name">{{name}}</span>
        <span class="handle">{{handle}}</span>
    </span>
</template>