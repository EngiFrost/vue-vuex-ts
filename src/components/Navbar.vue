<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router";

interface Route {
  link: string,
  title: string,
}

const routes: Route[] = [
  { link: '/', title: "Todos" }
];
</script>

<template>
  <nav id="navbar">
    <div id="btn-wrapper" v-for="route in routes">
      <RouterLink to="{{route.link}}">{{ route.title }}</RouterLink>A
    </div>
  </nav>
</template>

<style>
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
