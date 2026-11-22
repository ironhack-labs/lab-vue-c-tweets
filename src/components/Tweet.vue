<template>
  <div class="tweet">
    <ProfileImage :image="tweet.user.image" />
    <div class="body">
      <div class="top">
        <User :user-data="tweet.user" />
        <Timestamp :time="tweet.timestamp" />
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
import Timestamp from "./Timestamp.vue";
import User from "./User.vue";

defineProps({
  tweet: {
    type: Object,
    required: true,
  },
});
</script>
