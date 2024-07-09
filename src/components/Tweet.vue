<script setup>
import Actions from "./Actions.vue"
import LoMessage from "./Message.vue";
import User from "./user.vue";
import ProfileImage from "./ProfileImage.vue";
import Timestamp from './TimeStamp.vue';


defineProps({
  tweet: Object,
});


</script>


<template>
<div class="tweet">

    <img :src="tweet.user.image"
    class="profile"
      alt="profile"
    />

    <div class="body">
      <div class="top">
        <span class="timestamp">{{tweet.timestamp }}    </span>
        <span class="user"></span>
        <span class="name">{{tweet.user.name}} </span>
        <span class="handle">@{{tweet.user.handle}} </span>
        </div>

      <p class="message">
        {{tweet.message }}
      </p>

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
