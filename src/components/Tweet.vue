<template>
  <div class="tweet">
    <ProfileImage :image="user.image" />

    <div class="body">
      <div class="top">
        <User :userData="user"></User>
        <Timestamp :time="timestamp" />
      </div>
      <Message :message="message" />
      <Actions />
    </div>
    <!-- <span class="timestamp"></span>
      </div>

      <p class="message">
        
      </p>

      <div class="actions">
        <i class="far fa-comment"></i>
        <i class="fas fa-retweet"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-share"></i>-->

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>

<script setup>
import ProfileImage from './ProfileImage.vue';
import User from './User.vue';
import Timestamp from './Timestamp.vue';
import Message from './Message.vue';
import Actions from './Actions.vue';

const props = defineProps({
  tweet: {
    type: Object,
    required: true,
  },
});

const { user, timestamp, message } = props.tweet;

/*const props = defineProps({
  name : {
    type: String,
    required: true
  },
  handle : {
    type: String,
    required: true
  },
  img : {
    type: String,
    required: true
  },
  timestamp : {
    type: String,
    required: true
  },
  message : {
    type: String,
    required: true
  }
})*/
</script>
