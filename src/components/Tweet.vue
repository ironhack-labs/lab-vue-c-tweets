<template>
  <div class="tweet">
    <!-- Profile Img-->
    <ProfileImage :tweetChildImg="tweetImg" />

    <div class="body">
      <div class="top">
        <!-- User Name-->
        <User :tweetChildUser="tweetName" :tweetChildHandle="tweetHandle" />
        <!-- Timestamp of Tweet-->
        <Timestamp :tweetChildTimestamp="tweetTimestamp" />
      </div>
      <!-- Message of Tweet-->
      <Message :tweetChildMessage="tweetMessage" />
      <!-- Icons of Action-->
      <Actions />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script setup>
import { ref, reactive, computed } from "vue";
import ProfileImage from "./childComps/ProfileImage.vue";
import User from "./childComps/User.vue";
import Timestamp from "./childComps/Timestamp.vue";
import Message from "./childComps/Message.vue";
import Actions from "./childComps/Actions.vue";

defineProps({
  tweetName: String,
  tweetMessage: String,
  tweetImg: String,
  tweetHandle: String,
  tweetTimestamp: String,
});
</script>
<style scoped>
a {
  color: #42b983;
}
</style>
