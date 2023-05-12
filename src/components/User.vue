<script setup>
    defineProps({
        userData: {
            type: Object,
        }.
    });
</script>
<template>
    <span className="user">
        <span className="name">{{userData.name}}</span>
        <span className="handle">@ USER_HANDLE</span>
    </span>
</template>