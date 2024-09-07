<script setup lang="ts">
import StarRating from 'vue-star-rating'

const rating = defineModel() 


</script>

<template>
  <h2>Stars</h2>
  <star-rating v-model:rating="rating" :max-rating="5"></star-rating>

</template>

<style scoped>
</style>

