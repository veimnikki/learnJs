<template>
  <div id="app">
      <h1>Todo list</h1>
      <hr>
      <todoList 
      v-bind:todos="todos"
      />
  </div>
</template>

<script>
import todoList from '@/components/todoList'
export default {
  name: 'App',
  data() {
    return {
      todos: [
        {id: 1, title: 'Занятие спортом', completed: false},
        {id: 2, title: 'Медитация', completed: false},
        {id: 3, title: 'Саморазвитие', completed: false}
      ]
    }
  },
  components: {
    todoList
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
