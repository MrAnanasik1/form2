<template>
  <div id="app">
    <h1>to do</h1>
    <hr>
    <todolist 
      v-bind:todos="todos"
    />  
  </div>
</template>

<script>
import todolist from '@/components/todolist'

export default {
  name: 'app',
  data() {
    return {
      todos: [
        {id: 1, title: 'Купить хлеб',  completed: false},
        {id: 2, title: 'Купить масло',  completed: false},
        {id: 3, title: 'Купить пиво',  completed: false}
      ]
    }
  },
  components: {
    todolist
  }
}
</script>

<style>
</style>
