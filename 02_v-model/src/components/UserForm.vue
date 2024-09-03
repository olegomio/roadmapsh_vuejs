<script setup>
  const upName = defineModel()
  const upAge = defineModel()
</script>

<template>

  <form>
    <label>Name</label>
    <input type="text" v-model="upName" /> 
    
    <label>Alter</label>
    <input type="text" v-model="upAge" />
  </form>

</template>
