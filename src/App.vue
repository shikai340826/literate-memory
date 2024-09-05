<template>
  <div>
    <h2>{{ sum }}</h2>
    <button @click="increment">点击加一</button>
  </div>
</template>

<script setup lang='ts'>
  import { ref, reactive } from 'vue'
  let sum = ref(0);
  function increment() {
    sum.value += 1;
  }
</script>

<style scoped>
  h2{
    color: green;
  }
</style>