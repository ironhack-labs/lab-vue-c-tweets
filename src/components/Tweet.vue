<template>
  <header>
    <h2>Hello!</h2>
  </header>
  <div class="tweet">
    <ProfileImage :image="tweet.user.image" />

    <div>
      <h3 class="name"><User :user="tweet.user.name"/></h3>
      <p class="timestamp"><User :user="tweet.user.handle"/> . <Timestamp :time="tweet.timestamp"/></p>
      
      <Message :message="tweet.message"/>
    </div>
  </div>


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
      </p> -->
      

      <Actions />

</template>

<style scoped>
a {
  color: #42b983;
}
</style>

<script setup>

import Actions from "./Actions.vue";
import Message from "./Message.vue";
import ProfileImage from "./ProfileImage.vue"
import Timestamp from "./Timestamp.vue";
import User from "./User.vue";


defineProps({
  tweet: Object,
})
</script>
