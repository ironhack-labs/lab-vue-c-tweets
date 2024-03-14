<script setup>
const props = defineProps({
    message: String
})

const message = props.message

</script>

<template>

    <p class="message">
        {{ message }}
    </p>
</template>