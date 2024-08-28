<template>
    <div class="actions">
      <!-- Font Awesome icons -->
      <i class="far fa-comment"></i>
      <i class="fas fa-retweet"></i>
      <i class="far fa-heart"></i>
      <i class="fas fa-share"></i>
    </div>
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
  <style scoped></style>
  