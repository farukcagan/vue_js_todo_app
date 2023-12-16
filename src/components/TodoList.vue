<template>
  <div>
    <h1>Todo List</h1>
    <ul>
      <li v-for="todo in todos" :key="todo.id">{{ todo.title }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      todos: [],
    };
  },
  mounted() {
    fetch("https://jsonplaceholder.typicode.com/todos")
      .then((res) => res.json())
      .then((data) => {
        console.log(data);
        this.todos = data;
      })
      .catch((error) => {
        console.error("veri çekme hatası:", error);
      });
  },
};
</script>

<style scoped>
div{
    height: 500px;
}
li {
  background-color: rgb(186, 255, 250);
  margin-top: 5px;
  padding: 20px;
}
</style>
