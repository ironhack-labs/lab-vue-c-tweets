<template>
    <span>
    <span class="message">{{ text }}</span>
    
    </span>

  </template>
  
  <script>
 export default {
  name: 'Message',
  props: {
    text: {
      type: String,
      required: true
    }
  }
}
  </script>