<script setup>
    defineProps({
        userData: Object
    });
</script>

<template>
    <div class="user">
          <span class="name">{{ userData.name }}</span>
          <span class="handle">@{{ userData.handle }}</span>
    </div>
</template>