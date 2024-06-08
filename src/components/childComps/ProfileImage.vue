<!-- HTML -->
<template>
  <img
    :src="tweetChildImg"
    class="profile"
    :alt="`Image of the profile ${tweetChildName}`" />
</template>

<!-- JS  -->
<script setup>
import { ref, reactive, computed } from "vue";

defineProps({
  tweetChildImg: String,
  tweetChildName: String,
});
</script>
