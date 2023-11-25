<script>
  import AddForm from "./lib/AddForm.svelte";
  import ListaTodo from "./lib/ListaTodo.svelte";
  import TodoCounter from "./lib/TodoCounter.svelte";
  import {todos} from "./lib/store";
</script>

<main> 
  <h1>TODO List App</h1>
  <TodoCounter />
  <AddForm />
  <ListaTodo todoList={$todos} />
</main>

<style>
</style>
