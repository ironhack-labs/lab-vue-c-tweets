<script setup>

import ProfileImage from '@/components/ProfileImage.vue';
import User from '@/components/User.vue';
import Message from '@/components/Message.vue';
import Actions from '@/components/Actions.vue';
import Timestamp from '@/components/Timestamp.vue';

const props = defineProps({
  tweet: {
    type: Object,
    required: true
  }
});

</script>

<template>
  <div class="tweet">
    <ProfileImage :image="props.tweet.user.image"/>

    <div class="body">
      <div class="top">
        <User :userData="props.tweet.user"/>
<Timestamp :timestamp="props.tweet.timestamp"/>
      </div>
      <Message :message="props.tweet.message" />
      <Actions />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>