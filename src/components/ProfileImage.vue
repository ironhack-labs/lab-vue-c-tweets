<template>
  <img :src="img" class="profile" alt="profile" />
</template>

<script>
export default {
  name: "ProfileImage",
  props: {
    img: {
      type: String,
      required: true,
    },
  },
};
</script>
