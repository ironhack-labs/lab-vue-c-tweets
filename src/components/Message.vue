<script setup>

const props = defineProps({
  twMessage: {
    type: String,
    required: true
  }
});
</script>


<template>

    <p class="message"> {{ twMessage }}</p>

</template>