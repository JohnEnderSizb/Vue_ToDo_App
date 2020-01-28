<template>
  <div id="app">
    <Todo v-bind:todos="todos"/>
  </div>
</template>

<script>

  import Todo from './components/Todo.vue';

export default {
  name: 'app',
  components: {
    Todo
  },

  data() {
    return {
      todos: [
          {
              id:1,
              title: "To Do 1",
              completed: false
          },
              {
              id:2,
              title: "To Do 2",
              completed: true
          },
              {
              id:1,
              title: "To Do 3",
              completed: true
          },
              {
              id:1,
              title: "To Do41",
              completed: false
          }

      ]
    }
  }
}
</script>

<style>

  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

  body {
    font-family: Helvetica, Arial, sans-serif;
    line-height: 1.4;
  }

</style>
