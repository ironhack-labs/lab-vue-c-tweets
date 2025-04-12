<template>
    
    <span class="user">
    <span class="name">{{ userData.name }}</span>
    <span class="handle">@{{ userData.handle }}</span>
    </span>

  </template>
  
  <script>
 export default {
  name: 'User',
  props: {
    userData: {
      type: Object,
      required: true
    }
  }
}
  </script>