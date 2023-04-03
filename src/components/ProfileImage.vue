<template>
    <img :src="image" class="profile" alt="profile"/>
</template>

<script>
export default {
    name: 'ProfileImage',
    props: {
        image: {
            type: String,
            required: true,
        },
    },
}
</script>