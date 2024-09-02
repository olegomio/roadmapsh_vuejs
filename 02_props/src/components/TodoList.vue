<script setup>
import { ref } from 'vue'
import TodoItem from './TodoItem.vue'

</script>

<template>
  <ul>
    <TodoItem 
      v-for="item in items"
      :key="item.id"
      :title="item.title"
    />
  </ul>
</template>
