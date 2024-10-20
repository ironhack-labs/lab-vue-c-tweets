<script setup>
import ProfileImage from './ProfileImage.vue';
import User from './User.vue';
import Message from './Message.vue';
import TimeStamp from './Timestamp.vue';
import Actions from './Actions.vue';

defineProps(
  {
    tweet: Object
  }
);
</script>
<template>
  <div class="tweet">
    <ProfileImage v-bind:image=tweet.user.image />
    <div class="body">
      <div class="top">
        <User v-bind:user=tweet.user />
        <TimeStamp v-bind:timestamp=tweet.timestamp />
        
      </div>
      <Message v-bind:message=tweet.message></Message>
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
