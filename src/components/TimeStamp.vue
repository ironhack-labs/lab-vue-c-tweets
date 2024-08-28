<template>
    <span class="timestamp">{{ tweet.timestamp }}</span>
  </template>
  <script>
  export default {
    name: "TimeStamp",
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
  