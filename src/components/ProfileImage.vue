<template>
    
    <img :src="image" class="profile" :alt="alt" />
  </template>
  
  <script>
 export default {
  name: 'ProfileImage',
  props: {
    image: {
      type: String,
      required: true
    },
    alt: {
      type: String,
      default: 'profile'
    }
  }
}
  </script>
  
 
  