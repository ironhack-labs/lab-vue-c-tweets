# componente mostrará la fecha del tweet.
<script lang="ts" setup>
defineProps({
  TWEET_TIMESTAMP: String 
});
</script>

<template>
  <span>{{ date }}</span>
  <span class="timestamp">{{ TWEET_TIMESTAMP }}</span>
</template>

<style scoped>
span {
  color: gray;
  margin-left: 5px;
}
</style>
