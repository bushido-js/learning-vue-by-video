<template>
  <div id="app">
    <h1>Список</h1>
    <hr>
    <TodoList 
      v-bind:todos = 'todos'
    />
  </div>
</template>

<script>
import TodoList from "@/components/TodoList"
export default {
  name: 'App',
  data () {
    return {
      todos: [
        {id: 1, titel: 'Купить хлеб', completed: false},
        {id: 2, titel: 'Купить масло', completed: false},
        {id: 3, titel: 'Купить пиво', completed: false},
      ]
    }
  },
  components: {
    TodoList
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
