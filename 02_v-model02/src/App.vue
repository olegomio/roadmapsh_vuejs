<script setup lang="ts">
import Stars from './components/StarRating.vue'
import RatingDisplay from './components/RatingDisplay.vue'

import { ref } from 'vue'

const bewertung = ref(3)

</script>

<template>
	<h1>Rate Me!</h1><br />
	<Stars v-model="bewertung" /><br />
	<RatingDisplay :rate="bewertung" />

</template>

<style scoped>
</style>
