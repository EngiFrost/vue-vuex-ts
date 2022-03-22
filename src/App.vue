<script setup lang="ts">
import { RouterView } from "vue-router";
import Navbar from "./components/Navbar.vue";
</script>

<template>
  <main>
    <header id="main">
      <Navbar />
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
</style>
