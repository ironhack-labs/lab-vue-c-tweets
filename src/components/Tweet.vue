<script setup>
const props = defineProps(["tweet"]);
import ProfileImage from "./ProfileImage.vue";
import User from "./User.vue";
import Timestamp from "./Timestamp.vue";
import Message from "./Message.vue";
import Actions from "./Actions.vue";
</script>

<template>
  <div class="tweet">
    <ProfileImage :img="props.tweet.user.image" />
    <div class="body">
      <div class="top">
        <User :user="props.tweet.user"/>
        <Timestamp :time="props.tweet.timestamp" />
      </div>

      <Message :msg="props.tweet.message" />

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
