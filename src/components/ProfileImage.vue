<script>
const props = defineProps({
    image:src
})
</script>
<template>
    <img
      src={{image}}
      class="profile"
      alt="profile"
    />
</template>