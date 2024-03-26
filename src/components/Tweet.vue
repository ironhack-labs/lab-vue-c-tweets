<script setup>

const props = defineProps({
  user: {
    type: Object,
    name: { type: String },
    image: { type: String },
    handle: { type: String },
  },
  timestamp: { type: String },
  message: { type: String },
});
</script>

<template>
  <div class="tweet">
    <img :src="props.user.image" class="profile" alt="profile" />

    <div class="body">
      <div class="top">
        <span class="user">
          <span class="name">{{ props.user.name }}</span>
          <span class="handle">@{{ props.user.handle }}</span>
        </span>

        <span class="timestamp">{{ props.timestamp }}</span>
      </div>

      <p class="message">{{ props.message }}</p>

      <div class="actions">
        <!-- Font Awesome icons -->
        <i class="far fa-comment"></i>
        <i class="fas fa-retweet"></i>
        <i class="far fa-heart"></i>
        <i class="fas fa-share"></i>
      </div>
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>