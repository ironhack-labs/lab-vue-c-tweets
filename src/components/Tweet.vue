<script setup>
  import ProfileImage from './ProfileImage.vue';
  import User from './User.vue';
  import Timestamp from './Timestamp.vue';
  import Message from './Message.vue';
  import Actions from './Actions.vue';

  defineProps ({
    user: Object,
    message: String,
    timeStamp: String,
  })

</script>

<template>
  <div class="tweet">
    <ProfileImage :src="user.image" />

    <div class="body">
      <div class="top">
        <User :user="user" />
        <Timestamp :timeStamp="timeStamp" />
      </div>

      <Message :message="message"/>

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
