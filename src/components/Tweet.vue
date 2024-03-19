<script setup>

import User from './User.vue';
import ProfileImage from './ProfileImage.vue';
import Timestamp from './Timestamp.vue';
import Message from './Message.vue';
import Actions from './Actions.vue';

const props = defineProps({
  tweet: {
    type: Object,
    required: true
  }
});



</script>

<template>
  <div class="tweet">
    <ProfileImage :image="tweet.user.image"></ProfileImage>
    <div class="body">
      <div class="top">
        <span class="user">
          <User :username="tweet.user.name" :handle="tweet.user.handle"></User>
        </span>
        <Timestamp :timestamp="tweet.timestamp"></Timestamp>
      </div>

      <Message :message="tweet.message"></Message>

      <Actions> </Actions>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>
