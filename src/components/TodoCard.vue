<template>
  <div class="card">
    <div class="title">{{ props.todo.title }}</div>
    <Checkbox />
  </div>
</template>

<script setup lang="ts">
import type { Todo } from "../types/TodoTypes";
import Checkbox from "./TodoCheckbox.vue";

interface ITodoCardProps {
  todo: Todo;
}
const props = defineProps<ITodoCardProps>();
</script>

<style lang="scss" scoped>
.card {
  display: flex;
  justify-content: space-between;
  border: 2px solid black;
  width: fit-content;
  height: 20px;
  min-width: 100px;
  padding: 5px 5px 5px 10px;
  margin: 10px;
}
.title {
  font-size: 16px;
  font-weight: bold;
  &::first-letter {
    text-transform: uppercase;
  }
}
</style>
