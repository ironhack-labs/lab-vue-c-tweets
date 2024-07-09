<script setup>
import Time from "./TimeStamp.vue";

defineProps({
  user: Object,
  timeStamp: String,
});
</script>

<template >
<div class="top">
    <span class="user">
      <span class="name">{{ user.name }} </span>
      <span class="handle">@{{ user.handle }}</span>
    </span>

    <Time v-bind:timeStamp="timeStamp" />
  </div>  
</template>