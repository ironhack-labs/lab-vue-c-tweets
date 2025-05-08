<script setup>
import ProfileImage from "./ProfileImage.vue";
import User from "./User.vue";
import Message from "./Message.vue";
import Actions from "./Actions.vue";
import Timestemp from "./Timestamp.vue";

const props = defineProps({
  tweet: {
    user: {
      name: String,
      image: String,
      handle: String,
    },
    timestamp: String,
    message: String,
  },
});

const { tweet } = props;
const { user, timestamp, message } = tweet;
const { image } = user;
</script>

<template>
  <div class="tweet">
    <ProfileImage :image="image" />
    <div class="body">
      <div class="top">
        <User :user="user" />
        <Timestemp :time="timestamp" />
      </div>
      <Message :message="message" />
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
