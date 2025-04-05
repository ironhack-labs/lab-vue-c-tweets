<template>
  <div class="tweet" v-if="tweet">
    <ProfileImage :image="tweet.user.image" class="profile" />
  

    <div class="body">
      <div class="top">
        <User :userData="tweet.user" class="user" />
        <Timestamp :time="tweet.timestamp" class="timestamp" />
      </div>

      <Message :sms="tweet.message" class="message" />

      <Actions class="actions" />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script setup>
import { ref } from 'vue';
import ProfileImage from './ProfileImage.vue';
import User from './User.vue';
import Message from './Message.vue';
import Actions from './Actions.vue';
import Timestamp from './Timestamp.vue';

 
const props = defineProps({
  tweet: {
    type: Object
  }
});

</script>

<style scoped>
a {
  color: #42b983;
}
</style>
