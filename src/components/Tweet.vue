<template>
  <div class="tweet">
    <ProfileImage :image="tweet.user.image" />
    <div class="body">
      <div class="top">
        <span class="user">
          <span class="name">{{ tweet.user.name }}</span>
          <span class="handle">@{{ tweet.user.handle }}</span>
        </span>
        <Timestamp :time="tweet.timestamp" />
      </div>

      <Message :content="tweet.message" />

      <!-- Usar el componente Actions y manejar el evento -->
      <Actions @action="handleAction" />

    </div>
    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script setup>
import { defineProps } from 'vue';
import ProfileImage from './ProfileImage.vue';
import Timestamp from './Timestamp.vue';
import Message from './Message.vue';
import Actions from './Actions.vue'; // Importar el componente Actions

const props = defineProps({
  tweet: {
    type: Object,
    required: true
  }
});

// Manejar la acción emitida desde Actions
const handleAction = (actionType) => {
  console.log(`Acción realizada: ${actionType}`); // Aquí puedes manejar la acción como desees
};
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
