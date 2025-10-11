
<template>
<span class="timestamp">{{ time }}</span>

</template>


<script setup>
    defineProps({
  time: String
})
</script>

<style scoped>
.timestamp {
  color: gray;
  font-size: 0.9em;
}
</style>