<template>
  <div id="app">
    <div class="nav"><NavBar /></div>
    <div class="todo"><TodoList /></div>
  </div>
</template>

<script>
import TodoList from "./components/TodoList.vue";
import NavBar from "./components/NavBar.vue";

export default {
  name: "App",
  components: {
    NavBar,
    TodoList,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.todo{
  margin-top: 15px;
}
</style>
