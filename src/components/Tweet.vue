<script setup>
import { defineProps } from 'vue';
import User from '../components/User.vue';
import ProfileImage from '../components/ProfileImage.vue';
import Timestamp from '../components/Timestamp.vue';
import Message from '../components/Message.vue';
import Actions from '../components/Actions.vue';

const props = defineProps({
  tweet: {
    type: Object,
    required: true
  }
});
</script>

<template>
  <div class="tweet">
    <ProfileImage :image="tweet.user.image" />

    <div class="body">
      <div class="top">
        <User :userData="tweet.user" :userHandle="tweet.handle" />
        <Timestamp :time="tweet.timestamp" />
      </div>

      <Message :message="tweet.message" />
      <Actions />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>
