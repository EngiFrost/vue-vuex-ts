<template>
  <div class="board">
    <AddTodoForm />
    <TodoCard :todo="todo" />
  </div>
</template>

<script setup lang="ts">
import type { Todo } from "@/types/TodoTypes";
import AddTodoForm from "@/components/AddTodoForm.vue";
import TodoCard from "@/components/TodoCard.vue";
const todo: Todo = {
  id: "1",
  title: "test",
  content: "test",
};
</script>

<style scoped>
.board {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  border: 3px solid rgb(20, 89, 180);
  align-items: center;
  justify-content: center;
}
</style>
