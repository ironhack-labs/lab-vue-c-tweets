<script setup>

const props = defineProps({
    userData: {
        type: Object,
        required: true
    },
})

const { name, handle} = props.userData

</script>

<template>
    <span class="user">
    <span class="name">{{ name }}</span>
    <span class="handle">@{{ handle }}</span>
    </span>
</template>

<style scoped>

.name {
    font-weight: bold;
    margin-bottom: 0.5em;
    margin-right: 0.3em;
  }

  .handle {
    color: #536471;
    margin-left: 3px;
    margin-right: 3px;
  }
</style>