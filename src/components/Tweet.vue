<script setup>
import { defineProps } from 'vue';
import Actions from './Actions.vue';
import Message from './Message.vue';
import ProfileImage from './ProfileImage.vue';
import Timestamp from './Timestamp.vue';
import User from './User.vue';

// Definimos los props que vamos a recibir.
// Fíjate que aquí pone "movies", por lo tanto, cuando pasemos por prop en App.vue los datos deberemos referenciarlos como "movies".
const props = defineProps({
  tweetsP: {
    type: Array,
    required: true,
  }
})
</script>

<template>
  <div class="tweet" v-for="(tweet, index) in tweetsP" :key="index">
    <ProfileImage :image="tweet.user.image"></ProfileImage>
    
    <div class="body">
      <div class="top">
      <User :user="tweet.user"></User>
      <Timestamp :timestamp="tweet.timestamp"></Timestamp>
      </div>

      <Message :message ="tweet.message"></Message>
     <Actions class="actions"></Actions>

    </div>
  </div>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>
