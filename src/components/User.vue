# componente mostrará el nombre del usuario y su handle de Twitter.
<script lang="ts" setup>
defineProps({
  userData: Object 
});
</script>

<template>
 
 <div class="user">
  <span class="user">
    <span class="name">{{ userData.name }}</span>
    <span class="handle">{{ userData.twitterHandle }}</span> <!-- Mostrar el handle directamente -->
  </span>
  </div>

</template>

<style scoped>
.user-info {
  display: flex;
  align-items: center;
}



.handle {
  color: gray;
}
</style>
