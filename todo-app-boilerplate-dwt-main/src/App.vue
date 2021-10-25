<template>
  <main>
    <h1>Vue Todo List</h1>
    <VTitle>Vue Todo List</VTitle>

    <VTodoAdd />

    <ul class="todo-list">
      <VTodoItem />
    </ul>
  </main>
</template>

<script>
import VTitle from './components/VTitle'
import VTodoAdd from './components/VTodoAdd'
import VTodoItem from './components/VTodoItem'

export default {
  name: 'App',
  components: {
    VTodoItem,
    VTodoAdd,
    VTitle
  },

  setup () {
    return {}
  }
}
</script>

<style lang="scss">
* {
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  max-width: 500px;
  margin: 0 auto;
}

.todo-list {
  background: #ccc;
  border-radius: 5px;
  padding: 10px;
  display: flex;
  flex-direction: column;
  gap: 10px;
}
</style>
