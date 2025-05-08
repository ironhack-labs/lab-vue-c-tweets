<!-- src/components/Tweet.vue -->
<template>
  <div class="tweet">
    <ProfileImage :src="tweet.user.image" />
    <div class="body">
      <User
        :name="tweet.user.name"
        :handle="tweet.user.handle"
        :timestamp="tweet.timestamp"
      />
      <Message :content="tweet.message" />
      <Actions />
    </div>
  </div>
</template>

<script setup>
import ProfileImage from './ProfileImage.vue'
import User from './User.vue'
import Message from './Message.vue'
import Actions from './Actions.vue'

defineProps({
  tweet: {
    type: Object,
    required: true
  }
})
</script>

<style scoped>
.tweet {
  display: flex;
  gap: 1rem;
  padding: 1rem;
  border-bottom: 1px solid #ccc;
}
.body {
  flex: 1;
}
.message {
  margin: 0.5rem 0;
}
.actions {
  display: flex;
  gap: 1rem;
  font-size: 1.2em;
  color: gray;
}
</style>





