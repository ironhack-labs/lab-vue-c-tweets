<template>
  <span class="user">
    <span class="name">>{{ tweet.user.name }}</span>
    <span class="handle">{{ tweet.user.handle }}</span>
  </span>
</template>
<script>
export default {
  name: "User",
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
