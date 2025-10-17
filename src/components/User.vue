<template>
  <span class="user">
    <span class="name">{{ userData.name }}</span>
    <span class="handle">@{{ userData.handle }}</span>
  </span>
</template>

<script setup>
defineProps({
  userData: Object
});
</script>


<style scoped>
.name {
  font-weight: bold;
  margin-right: 0.3em;
}
.handle {
  color: #657786;
}
</style>
