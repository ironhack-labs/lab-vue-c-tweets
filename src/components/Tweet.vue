<template>
  <div class="tweet">
    <!-- Imagen de perfil del usuario -->
    <ProfileImage :image="tweet.user.image" />

    <div class="body">
      <div class="top">
        <!-- Información del usuario -->
        <User :user="tweet.user" />

        <!-- Timestamp del tweet -->
        <Timestamp :time="tweet.timestamp" />
      </div>

      <!-- Mensaje del tweet -->
      <Message :message="tweet.message" />

      <!-- Iconos de acciones -->
      <div class="actions">
        <i class="far fa-comment"></i>
        <i class="fas fa-retweet"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-share"></i>
      </div>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>


<script setup>
  import ProfileImage from './ProfileImage.vue';
  import User from './User.vue';
  import Timestamp from './Timestamp.vue';
  import Message from './Message.vue';

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
