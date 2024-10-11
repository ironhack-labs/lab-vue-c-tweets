# componente se encargará de mostrar el contenido del tweet.
<script lang="ts" setup>
defineProps({
  message: String
});
</script>

<template>
 <p class="message"> {{ message }}</p>
</template>

<style scoped>
p {
  margin: 10px 0;
}
</style>
