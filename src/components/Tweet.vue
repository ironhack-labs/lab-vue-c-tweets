<script setup>

import { defineProps } from 'vue';
import ProfileImage from './ProfileImage.vue';
import Timestamp from './Timestamp.vue';
import User from './User.vue';
import Message from './Message.vue';
import Actions from './Actions.vue';

defineProps({
  img: String,
  name: String,
  handle: String,
  timestamp: String,
  message: String,
})

</script>

<template>
  <div class="tweet">
    <ProfileImage
      :img="img"
      class="profile"> </ProfileImage>

    <div class="body">
      <div class="top">
        <span class="user">
          <User :name="name" :handle="handle" />
        </span>
        <Timestamp  
          :timestamp="timestamp"
          class="timestamp">
        </Timestamp>
      </div>

      <Message
        :message="message"
        class="message">
      </Message>

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
