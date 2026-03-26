<template>
  <div>
    <h2>{{ count }}</h2>
    <p>{{ message }}</p>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const count = ref(0)
const message = ref("Xin chào Vue!")
</script>

<style scoped>
h2 {
  color: red;
}
</style>

