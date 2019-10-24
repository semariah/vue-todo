<template>
  <div>
    <div v-for="todo in todos"></div>
    <h1>{{todo.title}}<h1>
  </div>
</template>

<script>
export default {
  name: "Todos",
  props: ["todos"]
};
</script>

<style scoped>
.todo-item {
  background: #f4f4f4;
  padding: 10px;
  border-bottom: 1px #ccc dotted;
}
.is-complete {
  text-decoration: line-through;
}
</style>