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
  border: 2px solid black;
  align-items: center;
  justify-content: flex-start;
  min-height: 100px;
  max-width: fit-content;
  padding: 5px;
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
