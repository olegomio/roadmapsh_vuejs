<script setup>

import UserForm from './UserForm.vue'

const props = defineProps({
  nameChange: String,
  ageChange: Number
});

</script>

<template>

  <h1>Display</h1>
  <div>
    <span>Name</span><br />
    <span>{{ nameChange }}</span>
  </div>
  <div>
    <span>Alter</span><br />
    <span>{{ ageChange }}</span>
  </div>

</template>
