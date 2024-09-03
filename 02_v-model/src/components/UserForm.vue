<script setup>
//  const upName = defineModel()
//  const upAge = defineModel()
defineEmits(['update:userNameChange', 'update:userAgeChange'])

let name = ''
let age = 0

function updateName(newName) {
  emit('update:userNameChange', newName);
}

function updateAge(newAge) {
  emit('update:userAgeChange', newAge);
}

</script>

<template>
  <h2>Form</h2>
  <form>
    <label>Name</label>
    <input type="text" v-model="name" @input="updateName($event.target.value)" /> 
    
    <label>Alter</label>
    <input type="number" v-model="age" @input="updateAge($event.target.value)" />
  </form>

</template>
