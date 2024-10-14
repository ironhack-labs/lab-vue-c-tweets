<template>
  <div class="tweet">
    <ProfileImage :image="tweet.user.image" />

    <div class="body">
      <div class="top">
        <User :user="tweet.user" />
        <Timestamp :time="tweet.timestamp" />
      </div>

      <p class="message">{{ tweet.message }}</p>

      <!-- Reemplaza los íconos con el componente Actions -->
      <Actions />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script setup>
  import ProfileImage from './ProfileImage.vue';
  import User from './User.vue';
  import Timestamp from './Timestamp.vue';
  import Message from './Message.vue';
  import Actions from './Actions.vue';

  // Definir la prop 'tweet'
  defineProps({
    tweet: Object
  });
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
