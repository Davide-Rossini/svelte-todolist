<script>
    import {todos} from "./store";

    let nuovoTodo 

    function AddTodo(){
        todos.update((old) =>{
            old.push({
                title: nuovoTodo,
                done: false
            })
            return old
        })
    }
</script>

<input type = "text" bind:value={nuovoTodo} class="input input-bordered input-info w-full max-w-xs"/>
<button on:click={AddTodo} class="btn btn-outline btn-primary">Add</button>