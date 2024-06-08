<!-- HTML -->
<template>
  <span class="user">
    <span class="name"> {{ tweetChildUser }} </span>
    <span class="handle">{{ tweetChildHandle }}</span>
  </span>
</template>

<!-- JS  -->
<script setup>
import { ref, reactive, computed } from "vue";

defineProps({
  tweetChildUser: String,
  tweetChildHandle: String,
});
</script>
