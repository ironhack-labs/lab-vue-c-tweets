<script setup>
import ProfileImage from '../components/ProfileImage.vue';
import User from '../components/User.vue'
import Timestamp from '../components/Timestamp.vue';
defineProps({
  tweet: Object
})
</script>

<template>
  <div class="tweet">

    <ProfileImage :image="tweet.user.image" />

    <div class="body">
      <div class="top">
        <User :userData="tweet.user" />
        <Timestamp :time="tweet.timestamp" />
      </div>

      <p class="message">
        {{ tweet.message }}
      </p>

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

<style scoped>
a {
  color: #42b983;
}
</style>
