<script setup>
import ProfileImage from '@/components/ProfileImage.vue';
import User from '@/components/User.vue';
import Timestamp from '@/components/Timestamp.vue';
import Message from '@/components/Message.vue';
import Actions from '@/components/Actions.vue';

defineProps({
  tweet: Object,
})
</script>

<template>
  <div class="tweet">
    <ProfileImage :image="tweet.user.image" />

    <div class="body">
      <div class="top">
        <User :user="tweet.user" />
        <Timestamp :timestamp="tweet.timestamp" />
      </div>
      <Message :message="tweet.message" />
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
