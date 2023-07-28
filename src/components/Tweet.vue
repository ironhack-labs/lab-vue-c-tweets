<template>

  <div class="tweet">
      <ProfileImage :image="props.userarray.user.image" />

      <div class="body">
          <div class="top">
              <User :userData="props.userarray.user" />
              <Timestamp :time="props.userarray.timestamp" />
          </div>

          <Message :message="props.userarray.message" />
          <Actions />
      </div>

      <i class="fas fa-ellipsis-h"></i>
  </div>

</template>

<script setup>

import { defineProps } from "vue";
import ProfileImage from "./ProfileImage.vue";
import User from "./User.vue";
import Timestamp from "./Timestamp.vue";
import Message from "./Message.vue";
import Actions from "./Actions.vue";


const props = defineProps({
  userarray: {
      type: Object,
      required: true,
      default: "missing data",
  },
});

</script>

<style>

a {
  color: #42b983;
}

</style>