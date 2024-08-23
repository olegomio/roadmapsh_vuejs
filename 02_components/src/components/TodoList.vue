<template>
	<div class="todo-list">
		<h2>My Todo List</h2>
		<input v-model="newTask" placeholder="Add a new task" @keyup.enter="addTask" />
		<button @click="addTask">Add Task</button>

		<ul>
			<li v-for="(task, index) in tasks" :key="index">
				<input type="checkbox" v-model="task.completed" />
				<span :class="{ 'completed: task.completed }">{{ task.text }}</span>
				<button @click="removeTask(index)">Remove</button>
			</li>
		</ul>
	</div>
</template>

<script>
export default {
	data() {
		return {
			newTask: '',
			tasks: [
				{ text: 'Learn Vue.js', completed: false },
				{ text: 'Build a todo list', completed: false }
			]
		};
	},
	methods: {
		addTask() {
			if (this.newTask.trim() !== '') {
				this.tasks.push({ text: this.newTask.trim(), completed: false });
				this.newTask = '';
			}
		},
		removeTask(index) {
			this.tasks.splice(index, 1);
		}
	}
};
</script>

<style scoped>
.todo-list {
	max-width: 400px;
	margin: auto;
	text-align: center;
}
.completed {
	text-decoration: line-through;
}
</style>
