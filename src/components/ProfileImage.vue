<template>
    <img :src="tweet.user.image" alt="User Image" class="user-image" />
  </template>
  <script>
  export default {
    name: "ProfileImage",
    props: {
      tweet: {
        type: Object,
        required: true,
      },
    },
  };
  </script>
  <style scoped>
  a {
    color: #42b983;
  }
  .user-image {
    border-radius: 50px;
    width: 80px;
    height: 80px;
  }
  </style>
  