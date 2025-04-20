<script setup>

import User from '../components/User.vue'
import Actions from '../components/Actions.vue'
import Message from '../components/Message.vue'
import ProfileImage from '../components/ProfileImage.vue'
import Timestamp from '../components/Timestamp.vue'

const props = defineProps({
  user: {
  name: String,
  img: String,
  handle: String,
  },  
  timestamp: String, 
  message: String,
});

</script>

<template>
  <div class="tweet">
    <ProfileImage image="user.image" />

    <div class="body">
      <div class="top">
        <User userData="user" />
        <Timestamp time="timestamp" />
      </div>

      <Message message="message" />
      <Actions />
    </div>
  <i class="fas fa-ellipsis-h"></i>

</div>
</template>


<!--
<script setup>
  
  const props = defineProps({
    name: String,
    img: String,
    handle: String,
    timestamp: String, 
    message: String,
  });

</script>

<template>
  <div class="tweet">
    <img
      src="https://i.imgur.com/9yw1Fyw.jpg"
      class="profile"
      alt="profile"
    />

    <div class="body">
      <div class="top">
        <span class="user">
          <span class="tweetname">{{name}}</span>
          <span class="handle">{{handle}}</span>
        </span>

        <span class="timestamp">{{timestamp}}</span>
      </div>

      <p class="message">
        {{message}}
      </p>

      <div class="actions">
     // Font Awesome icons 
        <i class="far fa-comment"></i>
        <i class="fas fa-retweet"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-share"></i>
      </div>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

-->

<style scoped>
a {
  color: #42b983;
}
</style>
