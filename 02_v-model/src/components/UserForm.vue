<script setup>
const name = defineModel('name')
const age = defineModel('age')
</script>

<template>
  <h2>Form</h2>
  <form>
    <label>Name</label>
    <input type="text" v-model="name" /> 
    
    <label>Alter</label>
    <input type="number" v-model="age" />
  </form>

</template>
