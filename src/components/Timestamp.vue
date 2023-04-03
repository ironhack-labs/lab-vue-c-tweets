<template>
 <span class="timestamp">{{time}}</span>
</template>

<script>
    export default {
        name: 'Timestamp',
        props: {
            time: {
                type: String,
                required: true,
            },
        },
    }
</script>