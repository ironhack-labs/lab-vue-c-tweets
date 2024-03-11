<script setup>
import { defineProps } from 'vue';

const props = defineProps({
  tweet: {
    type: Object,
    required: true
  }
});

const { timestamp, message, user } = props.tweet;
const { name, image, handle } = user;

</script>

<template>
  <div class="tweet">
    <img :src="image" class="profile" alt="profile" />

    <div class="body">
      <div class="top">
        <span class="user">
          <span class="name">{{ name }}</span>
          <span class="handle">{{ handle }}</span>
        </span>

        <span class="timestamp">{{ timestamp }}</span>
      </div>

      <p class="message">
        {{ message }}
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
