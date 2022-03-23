<template>
  <div class="wrapper">
    <form class="form">
      <input type="text" class="input" />
      <div class="btn-wrapper">
        <button class="button">Add</button>
        <button class="button">Clear checked</button>
      </div>
    </form>
  </div>
</template>

<script setup lang="ts"></script>

<style scoped>
.wrapper {
  display: flex;
  flex-direction: column;
  width: 300px;
  height: 50px;
}
.form {
  border: 1px solid black;
}
.input {
  width: 100%;
}

.btn-wrapper {
  display: flex;
  justify-content: space-between;
}
.button {
  border: 3px solid rgb(134, 134, 134);
}
</style>
