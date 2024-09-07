<script setup lang="ts">
import StarRating from 'vue-star-rating'
import { ref } from 'vue'


const rating = defineModel() 


</script>

<template>
  <h2>Stars</h2>
  <star-rating v-model:rating="rating" :rating="3" :max-rating="5"></star-rating>

</template>

<style scoped>
</style>

