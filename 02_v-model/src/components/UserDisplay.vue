<script setup>

import UserForm from './UserForm.vue'

const props = defineProps({
  name: String,
  age: Number
});

</script>

<template>

  <h1>Display</h1>
  <div>
    <span>Name</span><br />
    <span>{{ name }}</span>
  </div>
  <div>
    <span>Alter</span><br />
    <span>{{ age }}</span>
  </div>

</template>
