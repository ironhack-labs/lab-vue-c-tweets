<template>
  <section>
    <h2>Iteration 4: List of Tweets</h2>

    <div v-for="(tweet, index) in tweets" :key="index">
      <Tweet :tweet="tweet" />
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue'
import Tweet from './components/Tweet.vue'

const tweets = ref([
  {
    user: {
      name: 'Thoughts of Dog®',
      handle: '@dog_feelings',
      image: 'https://pbs.twimg.com/profile_images/1237550450/mstom_400x400.jpg'
    },
    timestamp: '1h ago',
    message:
      'the human likes to say. that i live here rent free. but i would argue. this housing accommodation. is my payment. for a lifetime of love. and excellent company'
  },
  {
    user: {
      name: 'Elon Musk',
      handle: '@elonmusk',
      image: 'https://pbs.twimg.com/profile_images/1590968738358079488/IY9Gx6Ok_400x400.jpg'
    },
    timestamp: '3h ago',
    message: 'Trump Sucks!'
  },
  {
    user: {
      name: 'NASA',
      handle: '@nasa',
      image: 'https://pbs.twimg.com/profile_images/1321163587679784960/0ZxKlEKB_400x400.jpg'
    },
    timestamp: '6h ago',
    message: 'Our Space program is shit '
  }
])
</script>

<style scoped>
section {
  width: 700px;
  margin: 30px auto;
  font-family: 'Helvetica Neue', Arial, sans-serif;
}
h2 {
  text-align: center;
  margin-bottom: 20px;
}
</style>
