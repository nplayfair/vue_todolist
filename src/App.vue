<template>
  <div id="app">
    <Todos v-bind:todos="todos" />
  </div>
</template>

<script>
import Todos from './components/Todos';

export default {
  name: 'app',
  components: {
    Todos
  },
  data() {
    return {
      todos: [
        {
          id: 1,
          title: "Item One",
          completed: false
        },
        {
          id: 2,
          title: "Item Two",
          completed: true
        },
        {
          id: 3,
          title: "Item Three",
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
