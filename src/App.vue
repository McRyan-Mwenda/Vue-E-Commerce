<script setup>
import { RouterView } from "vue-router";
import NavBar from "./components/NavBar.vue";
</script>

<template>
  <NavBar />

  <main class="home-view px-2">
    <RouterView />
  </main>

  <footer class="px-2 py-4">
    <div class="flex flex-row">
      <div></div>
      <div></div>
    </div>
    <div class="flex flex-row">
      <div></div>
      <div></div>
    </div>
  </footer>
</template>

<style scoped>
.home-view {
  min-height: 92vh !important;
}
</style>
