<script lang="ts" setup>
import ProfileImage from './ProfileImage.vue';
import User from './User.vue';
import Timestamp from './Timestamp.vue';
import Actions from './Actions.vue';
import Message from './Message.vue';

defineProps({
  tweet: Object
});
</script>
<template>
 
    
  <div class="tweet">
    <ProfileImage :image="tweet.user.profileImage" />

    <div class="body">
      <div class="top">
        <User :userData="tweet.user" />
        
        <Timestamp :TWEET_TIMESTAMP="tweet.date" />
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

.tweet {
  border: 1px solid #ddd;
  padding: 15px;
  border-radius: 10px;
  max-width: 600px;
  margin: 20px auto;
  background-color: #fff;
}


.header {
  display: flex;
  align-items: center;
}

.header img {
  margin-right: 10px;
}

.header div {
  display: flex;
  flex-direction: column;
}

.profile-img {
  width: 50px;
  height: 50px;
  border-radius: 50%;
  margin-right: 10px;
}

.user-info {
  display: flex;
  flex-direction: column;
}





.actions {
  display: flex;
  justify-content: space-around;
  margin-top: 10px;
}

button {
  background: none;
  border: none;
  cursor: pointer;
  font-size: 1.2em;
}
 
</style>



