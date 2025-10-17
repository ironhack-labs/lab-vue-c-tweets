<template>
  <div class="tweet">
    <ProfileImage :image="tweet.user.image" />

    <div class="body">
      <div class="top">
        <User :userData="tweet.user" />
        <Timestamp :time="tweet.timestamp" />
      </div>

      <Message :message="tweet.message" />
      <Actions />
    </div>


    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>


<script setup>
import ProfileImage from './ProfileImage.vue'
import User from './User.vue'
import Timestamp from './Timestamp.vue'
import Message from './Message.vue'
import Actions from './Actions.vue'

defineProps({
  tweet: Object
})
</script>

<style scoped>
.tweet {
  display: flex;
  border: 1px solid #e1e8ed;
  padding: 10px;
  margin: 10px auto;
  width: 600px;
  border-radius: 10px;
  background-color: #fff;
}

.body {
  margin-left: 10px;
  flex: 1;
}

.top {
  display: flex;
  align-items: center;
  margin-bottom: 5px;
}
</style>
