<script setup>
import { RouterView } from "vue-router";
import NavBar from "./components/NavBar.vue";
import PageFooter from "./components/PageFooter.vue";
</script>

<template>
  <NavBar />

  <main class="home-view px-2">
    <RouterView />
  </main>

  <PageFooter />
</template>

<style scoped>
.home-view {
  min-height: 92vh !important;
}
</style>
