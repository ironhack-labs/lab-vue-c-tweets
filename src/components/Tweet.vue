<script setup>
  const props = defineProps ({
    user: Object,
    message: String,
    timeStamp: String,
  })
  import ProfileImage from './ProfileImage.vue';
</script>

<template>
  <div class="tweet">
    <!-- <img :src="user.image" class="profile" alt="profile" /> -->
    <ProfileImage :src="user.image" />

    <div class="body">
      <div class="top">
        <span class="user">
          <span class="name">{{ user.name }}</span>
          <span class="handle">@{{ user.name }}</span>
        </span>

        <span class="timestamp">{{ timeStamp }}</span>
      </div>

      <p class="message">
        {{ message }}
      </p>

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

<style scoped>
a {
  color: #42b983;
}
</style>
