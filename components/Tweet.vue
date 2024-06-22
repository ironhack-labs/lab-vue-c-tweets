<template>
  <div class="tweet">
    <ProfileImage :image="tweet.user.image" />
    <div class="body">
      <div class="top">
        <div class="name"><User :name="tweet.user.name" /></div>
        <div class="handle">
          <User :handle="tweet.user.handle" />
        </div>
        <span class="timestamp">
          <Timestamp :timestamp="tweet.timestamp" />
        </span>
      </div>
      <p class="message">
        <Message :message="tweet.message" />
      </p>

      <div class="actions">
        <Actions />
      </div>
    </div>
    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script setup>
import { defineProps } from "vue";
import ProfileImage from "../components/ProfileImage.vue";
import User from "../components/User.vue";
import Timestamp from "../components/Timestamp.vue";
import Message from "../components/Message.vue";
import Actions from "../components/Actions.vue";

const props = defineProps({
  tweet: {
    type: Object,
    required: true,
  },
});
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
