<script setup>
import { ref, defineProps } from 'vue';
import ProfileImage from './ProfileImage.vue';
import User from './User.vue';
import Timestamp from './Timestamp.vue';
import Message from './Message.vue';
import Actions from './Actions.vue';

const props = defineProps({
 tweet: {
    type: Object,
    default: () => ({
      user: {
        name: "Ironhack",
        image: "https://i.imgur.com/9yw1Fyw.jpg",
        handle: "ironhack",
      },
      timestamp: "Nov 30, 2020",
      message: "On December 7th, we will be hosting a #webinar that will introduce you to #SQL! Are you ready? 🚀",
    }),
  },
});
</script>

<template>
  <div class="tweet">
    <ProfileImage :image="props.tweet.user.image" />

    <div class="body">
      <div class="top">
        <User :userData="props.tweet.user" />
        <Timestamp :time="props.tweet.timestamp" />
      </div>

      <Message :message="props.tweet.message" />
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
