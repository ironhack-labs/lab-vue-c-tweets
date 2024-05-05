<template>
  <div class="tweet">
    <ProfileImage :image="tweet.user.image" />
    <div class="body">
      <div class="top">
        <User :user="tweet.user" />
        <TimeStamp :timestamp="tweet.timestamp" />
      </div>
      <Message :message="tweet.message" />
      <Actions />
    </div>
    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script setup>
import Actions from "./Actions.vue";
import Message from "./Message.vue";
import ProfileImage from "./ProfileImage.vue";
import TimeStamp from "./TimeStamp.vue";
import User from "./User.vue";

import { defineProps } from "vue";
const props = defineProps({
  tweet: {
    user: Object,
    timestamp: String,
    message: String,

  },
});
//console.log(props.tweet);
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
