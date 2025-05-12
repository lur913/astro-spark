<template>
  <div class="text-3xl font-bold underline text-green-600 pt-3">{{ msg }}</div>
  <button @click="sayHello" class="bg-blue-500 text-white p-2 rounded-md cursor-pointer">say hello</button>
</template>

<script setup lang="ts">
import { ref } from 'vue'
const msg = ref('')
const sayHello = () => {
  if (msg.value === '') {
    msg.value = 'Hello, Vue!'
  } else {
    msg.value = ''
  }
}
</script>

<style scoped>

</style>