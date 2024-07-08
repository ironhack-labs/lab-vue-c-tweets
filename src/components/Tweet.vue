<script setup>
import ProfileImage from './ChildComponents/ProfileImage.vue';
import User from './ChildComponents/User.vue';
import TimeStamp from './ChildComponents/TimeStamp.vue';
import Message from './ChildComponents/Message.vue';
import Actions from './ChildComponents/Actions.vue';

defineProps({
  tweet: {type: Object, required: true,}
});
</script>

<template>
  <!-- src/App.vue -->
<!-- ... -->


  <!-- <div class="tweet">
    <img
      src="https://i.imgur.com/9yw1Fyw.jpg"
      class="profile"
      alt="profile"
    />

    <div class="body">
      <div class="top">
        <span class="user">
          <span class="name">Ironhack</span>
          <span class="handle">@ironhack</span>
        </span>

        <span class="timestamp">Nov 30, 2020</span>
      </div>

      <p class="message">
        On December 7th, we will be hosting a #webinar that will introduce you
        to #SQL! Are you ready? 🚀
      </p>  -->

        <!-- <div class="actions">
          Font Awesome icons 
         <i class="far fa-comment"></i>
        <i class="fas fa-retweet"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-share"></i>
      </div>
    </div> 

    <i class="fas fa-ellipsis-h"></i>
  </div> -->

  <div class="tweet">
    <ProfileImage :image="tweet.user.image" />
    <div class="body">
      <div class="top">
        <User :user="tweet.user" />
        <TimeStamp :timeStamp="tweet.timestamp" />
      </div>
      <Message :message="tweet.message" />
      <Actions />
  </div>
  <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<style scoped>

</style>
