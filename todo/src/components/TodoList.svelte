<script>
	import TodoItem from "./TodoItem.svelte";

	export let fetchTodos;
	export let handleCheckTodo;
	export let handleRemoveTodo;
	export let editMode;
	export let handleEditTodoItem;
	export let handleChangeEditMode;
</script>

<div class="main">
	<ul>
		{#each fetchTodos as todo, index (todo)}
			<li>
				<TodoItem {todo} {handleCheckTodo} {handleRemoveTodo} {editMode} {handleEditTodoItem} {handleChangeEditMode} />
			</li>
		{/each}
	</ul>
</div>
