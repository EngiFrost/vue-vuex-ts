<script setup lang="ts">
import { RouterLink } from "vue-router";

interface Route {
  link: string;
  title: string;
}

const routes: Route[] = [{ link: "/", title: "Todos" }];
</script>

<template>
  <nav id="navbar">
    <div id="btn-wrapper" v-for="(route, idx) in routes" :key="idx">
      <RouterLink to="{{route.link}}">{{ route.title }}</RouterLink>
    </div>
  </nav>
</template>

<style scoped>
#navbar {
  height: 60px;
  border: 4px solid rgb(8, 80, 104);
  display: flex;
  flex-direction: row-reverse;
  align-items: center;
  margin-bottom: 32px;
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
