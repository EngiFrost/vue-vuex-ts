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

<style scoped>
.form-wrapper {
  display: flex;
  flex-direction: column;
  width: 300px;
  height: 70px;
  border: 3px solid red;
}
.input {
  display: flex;
  box-sizing: border-box;
  width: 100%;
  height: 20px;
}

.btn-wrapper {
  display: flex;
  justify-content: space-around;
  height: 30px;
}
.button {
  border: 3px solid rgb(134, 134, 134);
  flex: 1;
}
</style>
