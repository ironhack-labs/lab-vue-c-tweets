<template>
    <p class="message">{{ message }}</p>
  </template>
  
  <script>
  export default {
    name: 'Message',
    props: {
      message: String
    }
  }
  </script>
  
  <style scoped>
  a {
    color: #42b983;
  }
  </style>
  