<template>
  <div class="tweet">
    <ProfileImage :img="tweet.user.image"></ProfileImage>

    <div class="body">
      <div class="top">
        <User :userData="tweet.user"></User>

        <Timestamp :timestamp="tweet.timestamp"></Timestamp>
      </div>

      <Message :message="tweet.message"></Message>

      <Actions></Actions>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script>
import ProfileImage from "./ProfileImage.vue";
import User from "./User.vue";
import Timestamp from "./Timestamp.vue";
import Message from "./Message.vue";
import Actions from "./Actions.vue";

export default {
  name: "Tweet",
  props: {
    tweet: {
      type: Object,
      required: true,
    },
  },
  components: {
    ProfileImage,
    User,
    Timestamp,
    Message,
    Actions,
  },
};
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
