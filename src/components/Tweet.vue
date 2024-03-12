<script setup>
import ProfileImage from './ProfileImage.vue';
import User from './User.vue';

const props = defineProps({
  tweet: {
    type: Object,
    required: true
  }
});

const { timestamp, message, user } = props.tweet;
const { image } = user;

</script>

<template>
  <div class="tweet">
    <ProfileImage :imageSrc="image" />

    <div class="body">
      <div class="top">
        <User :userData="user" />

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
