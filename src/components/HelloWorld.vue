<script setup>
import { ref } from "vue";

defineProps({
  msg: String,
});

const count = ref(0);
</script>

<template>
  <div class="prose">
    <li>dmeo</li>
  <h1>{{ msg }}</h1>
</div>
  <button
    class="bg-indigo-200 rounded m-2 p-2 flex justify-center"
    type="button"
    @click="count++"
  >
    count is {{ count }}
  </button>

</template>
