<script setup>
  import Tweet from '/src/components/Tweet.vue';

  const props = defineProps({
    image: String,
  
  })
</script>

<template>

    <img :src="image" alt="tweet.user.name" class="profile">

</template>


<style scoped>

</style>