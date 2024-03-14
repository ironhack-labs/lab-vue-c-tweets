<script setup>
import ProfileImage from "./ProfileImage.vue";
import User from "./User.vue";
import Timestamp from "./Timestamp.vue";
import Message from "./Message.vue";
import Actions from "./Actions.vue";

defineProps({
  tweet: {
    type: Object,
    required: true,
  },
});
</script>

<template>
  <div class="tweet">
    <ProfileImage :image="tweet.user.image" />

    <div class="body">
      <div class="top">
        <span class="user">
          <User :name="tweet.user.name" :handle="tweet.user.handle" />          
        </span>

        <Timestamp :timestamp="tweet.timestamp" />
      </div>

      <Message :message="tweet.message" />

      <div class="actions">
        <Actions />
      </div>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<!--  Iteration 1 ------------------------------------------------------
  
  <template>
  <div class="tweet">
    <img :src="props.tweet.user.image" class="profile" />

    <div class="body">
      <div class="top">
        <span class="user">
          <span class="name">{{ props.tweet.user.name }}</span>
          <span class="handle">{{ props.tweet.user.handle }}</span>
        </span>

        <span class="timestamp">{{ props.tweet.timestamp }}</span>
      </div>

      <p class="message">{{ props.tweet.message }}</p>

      <div class="actions">
        <i class="far fa-comment"></i>
        <i class="fas fa-retweet"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-share"></i>
      </div>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template> -->

<style scoped>
a {
  color: #42b983;
}
</style>
