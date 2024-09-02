<script setup>
defineProps(['item'])
</script>

<template>
  <li>
    <input type="checkbox">
    {{ item }}
  </li> 
</template>
