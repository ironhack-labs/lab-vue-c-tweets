<script setup>
// con esto vinculo todos los componentes que sirven a tweet.
import ProfileImage from './ProfileImage.vue'
import Timestamp from './Timestamp.vue'
import User from './User.vue'
import Message from './Message.vue'
import Actions from './Actions.vue'

// Aquí defino los props
const props = defineProps({
  tweet: {
    user: Object,
    timestamp: String,
    message: String
  }
})
</script>

<template>
  <div class="tweet">
    <!-- aqui se inyecta el componente ver ProfileImage col10+ -->
    <ProfileImage :image="tweet.user.image"></ProfileImage>
    <div class="body">
      <div class="top">
        <User :user="tweet.user"></User>   
        <Timestamp :timestamp="tweet.timestamp"></Timestamp>
      </div>
      <Message :message="tweet.message"></Message> 
      <Actions></Actions>
    </div>
    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>
