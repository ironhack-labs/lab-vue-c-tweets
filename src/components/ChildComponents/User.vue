<template>
    <span class="user">
          <span class="name">{{ user.name }}</span>
          <span class="handle">@{{ user.handle }}</span>
    </span> 
</template>

<script setup>

defineProps({
    user: Object,
});

</script>
