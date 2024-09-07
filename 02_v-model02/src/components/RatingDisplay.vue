<script setup lang="ts">

const props = defineProps({
  rate: Number
})

</script>


<template>
  <h2>RatingDisplay</h2>
  <span><span>{{ props.rate }}</span> von 5 Sternen</span>


</template>
