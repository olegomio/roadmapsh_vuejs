<script setup>
import { defineProps } from 'vue'
import TodoItem from './TodoItem.vue'

defineProps({
  items: {
    type: Array,
    required: true
  },
});
</script>

<template>
  <ul>
    <TodoItem 
      v-for="item in items"
      :key="item.key"
      :title="item.title"
    />
  </ul>
</template>
