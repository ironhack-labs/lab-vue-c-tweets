<template>
  <div class="tweet">
    <ProfileImage :src="image" />
    <!-- <img :src="image" class="profile" alt="profile" /> -->

    <div class="body">
      <div class="top">
        <User :name="name" :handle="handle" />

        <!-- <span class="user">
          <span class="name">
            {{ tweets }}</span>
          <span class="handle">@hj</span>
        </span> -->
        <Timestamp :timestamp="timestamp" />
        <!-- <span class="timestamp">jugj</span> -->

      </div>
      <Message :message="message" />
      <!-- <p class="message">
        {{ message }}
      </p> -->

      <Actions />
      <!-- <div class="actions">
        
        <i class="far fa-comment"></i>
        <i class="fas fa-retweet"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-share"></i>
      </div> -->
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>
<script setup>
import User from './User.vue'
import Timestamp from './Timestamp.vue'
import ProfileImage from './ProfileImage.vue';
import Message from './Message.vue';
import Actions from './Actions.vue';
import { ref } from 'vue';

const props = defineProps(['name', 'image', 'handle', 'timestamp', 'message', 'user']);

const actions = ref(['comment, retweet, heart, share'])

</script>

<style scoped>
a {
  color: #42b983;
}
</style>
