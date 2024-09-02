<script setup lang="ts">
import { ref } from 'vue';
import TodoList from './components/TodoList.vue'

const items = ref([
{ key: 1, title: 'todo 1' },
{ key: 2, title: 'todo 2' },
{ key: 3, title: 'todo 3' },
{ key: 4, title: 'todo 4' },
{ key: 5, title: 'todo 5' }
])
</script>

<template>
  <header>
    <div class="wrapper">
      <h1>Prop Excercise!</h1>
    </div>
  </header>

  <main>
    <TodoList :items="items" />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
