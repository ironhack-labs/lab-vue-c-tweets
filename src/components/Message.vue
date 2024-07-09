<script setup>
defineProps({
    message: String,
})
</script>

<template >
<p class="message">
        {{tweet.message }}
      </p>

</template>