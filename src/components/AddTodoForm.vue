<template>
  <div class="form-wrapper">
    <input type="text" class="input" />
    <input type="text" class="input" />
    <div class="btn-wrapper">
      <button class="button">Add</button>
      <button class="button">Clear checked</button>
    </div>
  </div>
</template>

<script setup lang="ts"></script>

<style lang="scss" scoped>
.form-wrapper {
  display: flex;
  flex-direction: column;
  width: 300px;
  border: 3px solid red;
}
.input {
  display: flex;
  box-sizing: border-box;
  width: 100%;
  height: 30px;
}

.btn-wrapper {
  display: flex;
  justify-content: space-around;
}
.button {
  border: 2px solid rgb(134, 134, 134);
  border-radius: 5px;
  height: 30px;
  width: 120px;
  margin: 5px;
  &:hover {
    background-color: lightgray;
  }
}
</style>
