<template>
  <div class="tweet">
       <ProfileImage :image="tweet.user.image" />


    <div class="body">
      <div class="top">
        <User :userData="tweet.user" />
        <Timestamp :time="tweet.timestamp" />

      </div>

        <Message :message="tweet.message" />

      <div class="actions">
        <!-- Font Awesome icons -->
        <i class="far fa-comment"></i>
        <i class="fas fa-retweet"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-share"></i>
      </div>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script setup>
import ProfileImage from './ProfileImage.vue';
import User from './User.vue';
import Timestamp from './Timestamp.vue';
import Message from './Message.vue';


defineProps({
    tweet: Object
})

</script>

<style scoped>
a {
  color: #42b983;
}
</style>
