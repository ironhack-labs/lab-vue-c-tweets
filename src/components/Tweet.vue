<script setup>
import Actions from "./TweetComps/Actions.vue";
import Message from "./TweetComps/BodyMessage.vue";
import User from "./TweetComps/User.vue";
import ProfileImage from "./TweetComps/ProfileImage.vue";

defineProps({
  tweet: Object,
});
</script>

<template>
  <div class="tweet">
    <ProfileImage v-bind:image="tweet.user.image" />

    <div class="body">
      <User v-bind:user="tweet.user" v-bind:timeStamp="tweet.timestamp" />
      <Message v-bind:message="tweet.message" />
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
