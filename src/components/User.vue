<script setup>
  import { defineProps } from 'vue';
  
  const props = defineProps({
    userData: {
      type: Object,
      required: true,
      validator: (value) => {
        return value.name && value.handle;
      },
    },
  });
  </script>
  
  <template>
    <span class="user">
      <span class="name">{{ userData.name }}</span>
      <span class="handle">@{{ userData.handle }}</span>
    </span>
  </template>

  <style scoped>
  </style>
  