<script setup lang="ts">
import UserDisplay from './components/UserDisplay.vue'
import UserForm from './components/UserForm.vue'
import { ref } from 'vue'

let UserName = "Mustermann"
let UserAge = 18

</script>

<template>

  <h1>V-Model Excercise</h1>

  <UserDisplay :nameChange='UserName' :ageChange='UserAge' />
  <UserForm @userNameChange="UserName = $event" @userAgeChange="UserAge = $event" />

</template>

<style scoped>
</style>
