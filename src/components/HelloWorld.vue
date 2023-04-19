<script setup>
import { ref } from 'vue';

defineProps({
  msg: String,
  icon: String,
  url: String,
});

const count = ref(0);
</script>

<template>
  <div class="flex justify-center items-center">
    <div class="prose">
      <h2>{{ msg }} {{ icon }}</h2>
      <a :href="url" target="_blank">bing.com</a>
      <button
        class="bg-indigo-200 rounded m-2 p-2"
        type="button"
        @click="count++"
      >
        count is {{ count }}
      </button>
    </div>
  </div>
</template>
