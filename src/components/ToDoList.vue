<template>
  <h1>Hello To Do List</h1>
</template>

<script>
    import { todoItems } from "../data";
    import TodoItem from "./TodoItem.vue"

    export default {
        components: {TodoItem},
        data() {    
            return {
                todos: [...todoItems],
            };
        },
    };
</script>

<style>

</style>