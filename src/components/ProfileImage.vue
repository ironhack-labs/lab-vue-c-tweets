# script sobre la imagen del perfil del usuario
<script lang="ts" setup>
defineProps({
  image: String
});
</script>

<template>
  
  <img :src="image" class="profile" alt="profile" />
</template>

<style scoped>
img {
  width: 50px;
  height: 50px;
  border-radius: 50%;
}

.profile {
  width: 50px;
  height: 50px;
  border-radius: 50%;
}
</style>
    
