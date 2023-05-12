<script setup>
    defineProps({
        time:{
            type: String,
        }
    });
</script>
<template>
    <span className="timestamp">{{time}}</span>
</template>