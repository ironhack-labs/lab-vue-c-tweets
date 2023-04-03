<template>
  <div class="tweet">
    <ProfileImage :image="tweet.user.image" />

    <div class="body">
      <div class="top">
        <User :name="tweet.user.name" :handle="tweet.user.handle" />
        <Timestamp :time="tweet.timestamp" />
      </div>

      <Message :message="tweet.message" />
      <Actions />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script>
import ProfileImage from './ProfileImage.vue'
import User from './User.vue'
import Timestamp from './Timestamp.vue'
import Message from './Message.vue'
import Actions from './Actions.vue'

export default {
  name: 'Tweet',
  props: {
    tweet: {
      user: Object,
      message: String,
      timestamp: String,
    }
  },
  components: {
    ProfileImage,
    User,
    Timestamp,
    Message,
    Actions,
  }
}
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
