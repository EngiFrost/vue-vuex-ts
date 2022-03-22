<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <main>
    <header id="main">
      <nav id="navbar">
        <div id="btn-wrapper">
          <RouterLink to="/">Todos</RouterLink>
        </div>
      </nav>
    </header>

    <RouterView />
  </main>
</template>

<style>
#app {
  max-width: 1280px;
  margin: 0 auto;
  padding: 2rem;
  border: 2px solid black;
  font-weight: normal;
}

#navbar {
  width: 100%;
  height: 60px;
  border: 4px solid rgb(8, 80, 104);
  display: flex;
  flex-direction: row-reverse;
  align-items: center;
}

#btn-wrapper {
  padding: 10px;
  border: 3px solid rgb(0, 62, 133);
  height: fit-content;
  width: fit-content;
  margin-right: 10px;
}

#btn-wrapper > a {
  text-transform: uppercase;
  font-size: 14px;
  font-weight: 700;
  text-decoration: none;
  color: black;
}
</style>
