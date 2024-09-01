<script setup>
  import { ref } from 'vue'
  const greeting = ref('geschafft du spasst')
</script>

<template>
  <p class="greeting">{{ greeting }}</p>
</template>

<style>
.greeting {
  color: red;
  font-weight: bold;
}
</style>
