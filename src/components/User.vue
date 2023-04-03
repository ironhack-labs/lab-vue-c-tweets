<template>
    <span class="user">
          <span class="name">{{ name }}</span>
          <span class="handle">@{{ handle }}</span>
        </span>
</template>

<script>
export default {
    name: 'User',
    props: {
        name: {
            type: String,
            required: true,
        },
        handle: {
            type: String,
            required: true,
        },    
    },
}    
</script>