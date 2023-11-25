<script>
  import TodoComponent from "./TodoComponent.svelte";

    export let todoList = [];
</script>

{#each todoList as todo, pos}
    <TodoComponent {todo} {pos}/>
{/each}