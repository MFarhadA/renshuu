<script setup lang="ts">
  const count = ref(0);

  function increment() {
    count.value++;
  }

  function decrement() {
    count.value--;
  }
</script>

<template>
  <div>
    <h3>Welcome to Nuxt 3</h3>
      <p>Count: {{ count }}</p>
      <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded" @click="increment">Increment</button>
      <button class="bg-red-500 hover:bg-red-700 text-white font-bold py-2 px-4 rounded" @click="decrement">Decrement</button>
  </div>
</template>