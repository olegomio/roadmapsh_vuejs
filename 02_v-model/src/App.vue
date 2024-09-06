<script setup lang="ts">
import UserDisplay from './components/UserDisplay.vue'
import UserForm from './components/UserForm.vue'
import { ref } from 'vue'

const name = ref('Max Mustermann')
const age = ref(18)

</script>

<template>

  <h1>V-Model Excercise</h1>

  <UserDisplay :name="name" :age="age" />
<UserForm v-model:name="name" v-model:age="age" />

</template>

<style scoped>
</style>
