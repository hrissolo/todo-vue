<template>
<div>
  <h1>Hello To Do List</h1>
     <div v-for="item in todos" :key="item.id">
      <todo-item :todo="item"/>
    </div>
</div>  
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