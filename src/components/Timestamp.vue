<template>
    <span>
    <span class="timestamp">{{ time }}</span>
    
    </span>

  </template>
  
  <script>
 export default {
  name: 'Timestamp',
  props: {
    time: {
      type: String,
      required: true
    }
  }
}
  </script>