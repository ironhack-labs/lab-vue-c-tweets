<template>
  <span class="timestamp">{{ time }}</span>
</template>

<script setup>
defineProps({
  time: String
});
</script>


<style scoped>
.timestamp {
  color: #657786;
  margin-left: 0.5em;
}
</style>
