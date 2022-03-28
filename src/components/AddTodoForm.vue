<template>
  <div class="form-wrapper">
    <input type="text" placeholder="Enter todo title" class="input" />
    <button class="button">Add</button>
    <button class="button">Clear checked</button>
  </div>
</template>

<script setup lang="ts"></script>

<style lang="scss" scoped>
.form-wrapper {
  display: flex;
  align-items: center;
  width: 400px;
  border: 2px solid red;
  margin: 40px 0;
}
.input {
  display: flex;
  flex: 1;
  box-sizing: border-box;
  height: 30px;
}
.button {
  border: 2px solid rgb(134, 134, 134);
  height: 30px;
  white-space: nowrap;
  &:hover {
    background-color: lightgray;
  }
}
</style>
