<template>
    <div class="tweet">
      <ProfileImage :tweet="tweet" />
  
      <div class="body">
        <div class="top">
          <User :tweet="tweet" />
          <TimeStamp :tweet="tweet" />
        </div>
  
        <Message :tweet="tweet" />
        <Actions :tweet="tweet" />
      </div>
  
      <i class="fas fa-ellipsis-h"></i>
    </div>
  </template>
  <script>
  import ProfileImage from "./ProfileImage.vue";
  import User from "./User.vue";
  import Message from "./Message.vue";
  import TimeStamp from "./TimeStamp.vue";
  import Actions from "./Actions.vue";
  export default {
    name: "Tweet",
    components: {
      ProfileImage,
      User,
      Message,
      TimeStamp,
      Actions,
    },
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
  