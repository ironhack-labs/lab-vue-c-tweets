<script setup>
  // Imports of components
  import ProfileImage from './ProfileImage.vue';
  import User from './User.vue';
  import Timestamp from './Timestamp.vue';
  import Message from './Message.vue';
  import Actions from './Actions.vue';


  // Props
  const props = defineProps({
    tweet: Object,
  });

  const name = props.tweet.user.name
  const handle = props.tweet.user.handle
  const image = props.tweet.user.image
  const timestamp = props.tweet.timestamp
  const message = props.tweet.message

</script>

<template>
  <div class="tweet">
    <ProfileImage :image="image"/>
    <div class="body">
      <div class="top">
        <User :name="name" :handle="handle"/>
        <Timestamp :timestamp="timestamp"/>
      </div>
      <Message :message="message"/>
      <Actions/>
    </div>
    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>
