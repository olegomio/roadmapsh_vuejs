<script setup>
defineProps({
  key: Number,
  title: String
})
</script>

<template>
  <li :id="key">
    <input type="checkbox">
    {{ title }}
  </li> 
</template>
