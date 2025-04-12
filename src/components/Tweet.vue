
<template>
 
  <div class="tweet">
    <ProfileImage :image="tweet.user.image" :alt="tweet.user.name" />
  

    <div class="body">
      <div class="top">
        <User :userData="tweet.user" />

        <Timestamp :time="tweet.timestamp" />
      </div>

      <Message :text="tweet.message"/>
        
      <div class="actions">
        <Actions />

      </div>
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


const props = defineProps({
  tweet: {
    type: Object,
    required: true,
  },
});
</script>


<style scoped>
a {
  color: #42b983;
}
</style>
