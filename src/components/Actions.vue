
<script setup>
  import { ref } from 'vue';


  const like = ref(false)
  const contador = ref(0)

  const isLiked = () => {
    like.value = !like.value

    if(like.value) {
      contador.value++
    }
    
    if(!like.value) {
      contador.value--
    }
    
    console.log(contador.value)
  }



</script>

<template>
  <div class="actions">
    <!-- Font Awesome icons -->
    <i class="far fa-comment"></i>
    <i class="fas fa-retweet"></i>
    <div class="container-contador">
      <i class="far fa-heart" :class="[like ? 'fas fa-heart like' : 'far fa-heart']" @click="isLiked"></i>
      <p>{{ contador }}</p>
    </div>
    <i class="fas fa-share"></i>
  </div>
</template>


<style scoped>
 .like {
  color: red;

 }

 .far.fa-heart:hover {
  cursor: pointer;

 }

 .container-contador {
  display: flex;
  gap: 20px;
  justify-content: flex-start;
  align-items: flex-start;

 }

 .container-contador p {
  margin: 0;
 }


</style>