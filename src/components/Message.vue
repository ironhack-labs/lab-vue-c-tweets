<template>
    <p class="message">
      {{ tweet.message }}
    </p>
  </template>
  <script>
  export default {
    name: "Message",
    props: {
      tweet: {
        type: Object,
        required: true,
      },
    },
  };
  </script>
  <style scoped></style>
  