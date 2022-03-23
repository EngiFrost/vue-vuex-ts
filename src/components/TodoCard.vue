<template>
  <div class="card">
    <div class="title">{{ props.todo.title }}</div>
    <div class="content">{{ props.todo.content }}</div>
  </div>
</template>

<script setup lang="ts">
import type { Todo } from "../types/TodoTypes";

interface ITodoCardProps {
  todo: Todo;
}
const props = defineProps<ITodoCardProps>();
</script>

<style scoped>
.card {
  display: flex;
  flex-direction: column;
  border: 2px solid black;
  align-items: center;
  justify-content: flex-start;
  height: fit-content;
  width: fit-content;
  min-height: 60px;
  min-width: 100px;
  padding: 5px;
  margin: 10px;
}
.title {
  font-size: 16px;
  font-weight: bold;
  text-decoration: underline;
}
.content {
  font-size: 12px;
}
</style>
