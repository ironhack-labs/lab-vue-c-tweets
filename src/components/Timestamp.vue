<template>
    <span class="timestamp">{{ time }}</span>
  </template>
  
  <script>
  export default {
    name: 'Timestamp',
    props: {
      time: String
    }
  }
  </script>
  
  <style scoped>
  a {
    color: #42b983;
  }
  </style>