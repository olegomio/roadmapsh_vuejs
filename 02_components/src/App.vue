<template>
	<div id="app">
		<TodoList />
		<SingleFileComponent />
	</div>	
</template>

<script>
	import TodoList from './components/TodoList.vue';
	import SingleFileComponent from './components/Single-File-Components.vue';

	export default {
		name: 'App',
		components: {
			TodoList,
			SingleFileComponent
		}
	};


</script>
