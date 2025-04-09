
<script setup>
  import { ref } from 'vue';
  import Tweet from './components/Tweet.vue';

  const tweets = ref([
    {
      user: {
        name: "Thoughts of Dog®",
        image: "https://i.imgur.com/b0EdHVV.jpg",
        handle: "dog_feelings",
      },
      timestamp: "1h ago",
      message: "the human likes to say. that i live here rent free. but i would argue. this housing accommodation. is my payment. for a lifetime of love. and excellent company",
    },
    {
      user: {
        name: "Thoughts of Dog®",
        image: "https://i.imgur.com/b0EdHVV.jpg",
        handle: "dog_feelings",
      },
      timestamp: "2h ago",
      message: "sometimes. the human presses their noggin against mine. to figure out what i’m thinking. so i just think really hard. about how much i love them. and hope they figure it out",
    },
    {
      user: {
        name: "Thoughts of Dog®",
        image: "https://i.imgur.com/b0EdHVV.jpg",
        handle: "dog_feelings",
      },
      timestamp: "3h ago",
      message: "here is what. i plan to accomplish today: \n\n2. bark loudly. but at nothing \n7. lose my ball under the couch\n7b. politely ask the human. to get my ball\n3. immediately lose it again. under the same couch\n4. big nap. you have worked hard\n2. repeat",
    }
]);



</script>

<template>
  <div class="app">
    <!-- agregando el componente Tweet con un prop llamado tweet al que le pases el primer objeto del array tweets -->
    <!-- Renderiza todos los tweets usando v-for -->
    <Tweet v-for="(tweet, index) in tweets" :key="index" :tweet="tweet" />
    <div class="brain-party" style="animation: brain-party 2s infinite;"></div>
  </div>


</template>

<style>
  body {
    margin: 0;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "Roboto", "Oxygen",
      "Ubuntu", "Cantarell", "Fira Sans", "Droid Sans", "Helvetica Neue",
      sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }

  .app {
    text-align: center;
  }

  .app-logo {
    height: 40vmin;
    pointer-events: none;
  }

  @media (prefers-reduced-motion: no-preference) {
    .app-logo {
      animation: App-logo-spin infinite 20s linear;
    }
  }

  .app-header {
    background-color: #282c34;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    font-size: calc(10px + 2vmin);
    color: white;
  }

  .app-link {
    color: #61dafb;
  }

  @keyframes App-logo-spin {
    from {
      transform: rotate(0deg);
    }
    to {
      transform: rotate(360deg);
    }
  }

  .app {
    padding: 20px;
  }

  .tweet {
    margin: 0 auto;
    min-width: 480px;
    max-width: 640px;
    min-height: 80px;
    padding: 10px;
    border: 1px solid #ccc;
    display: flex;
    font-size: 1.1rem;
    line-height: 18px;
  }

  .body {
    display: flex;
    flex-direction: column;
    width: 100%;
  }

  .top {
    display: flex;
    line-height: 1.4rem;
  }

  .more {
    margin-left: 20px;
  }

  .profile {
    width: 50px;
    height: 50px;
    border-radius: 50px;
    margin-right: 10px;
  }

  .name {
    font-weight: bold;
    margin-bottom: 0.5em;
    margin-right: 0.3em;
  }

  .handle {
    color: #536471;
    margin-left: 3px;
    margin-right: 3px;
  }

  .timestamp {
    color: #536471;
    font-size: 1.1rem;
  }

  .timestamp::before {
    content: "·";
    padding-right: 0.3em;
    font-size: 1.1rem;
    font-weight: 600;
  }

  .message {
    text-align: left;
    font-stretch: 100%;
    font-weight: 400;
    line-height: 1.6rem;
    overflow-wrap: break-word;
    white-space: pre-wrap;
  }

  .actions {
    padding: 5px 5px;
    width: 360px;
    display: flex;
    justify-content: space-between;
    color: #536471;
  }


  .brain-party {
  width: 100px;
  height: 20px;
  margin: 20px auto;
  border-radius: 10px;
  background: #42b983;
  animation: brain-party 1.5s infinite ease-in-out;
}

@keyframes brain-party {
  0% {
    background: #42b983;
    transform: scaleX(1);
  }
  50% {
    background: #35495e;
    transform: scaleX(1.2);
  }
  100% {
    background: #42b983;
    transform: scaleX(1);
  }
}


</style>