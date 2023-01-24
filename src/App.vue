<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <nav
    class="flex flex-row justify-between px-2 py-4 items-center backdrop-blur-sm bg-sky-700 text-lg text-gray-200"
  >
    <div class="flex flex-row items-center">
      <div class="mr-4">
        <RouterLink to="/" class="font-semibold text-xl hover:text-white"
          >Gadget shop</RouterLink
        >
      </div>
      <div class="dropdown relative">
        <RouterLink to="/" class="mr-4 hover:text-white"
          >Shop <i class="bi bi-caret-down-fill text-sm"></i
        ></RouterLink>
        <div
          class="dropdown-content absolute text-gray-600 py-2 px-4 rounded-md ddw-1"
        >
          <h1>something very long</h1>
          <h1>something very long</h1>
          <h1>something very long</h1>
          <h1>something very long</h1>
          <h1>something very long</h1>
          <h1>something very long</h1>
        </div>
      </div>
      <div class="dropdown relative">
        <RouterLink to="/" class="mr-4 hover:text-white"
          >Accounts <i class="bi bi-caret-down-fill text-sm"></i
        ></RouterLink>
        <div class="dropdown-content absolute text-gray-600 rounded-md ddw-2">
          <h1>something very long</h1>
          <h1>something very long</h1>
          <h1>something very long</h1>
          <h1>something very long</h1>
          <h1>something very long</h1>
          <h1>something very long</h1>
        </div>
      </div>
      <div class="dropdown relative">
        <RouterLink to="/" class="mr-4 hover:text-white"
          >More <i class="bi bi-caret-down-fill text-sm"></i
        ></RouterLink>
        <div class="dropdown-content absolute text-gray-600 rounded-md ddw-2">
          <h1>something very long</h1>
          <h1>something very long</h1>
          <h1>something very long</h1>
          <h1>something very long</h1>
          <h1>something very long</h1>
          <h1>something very long</h1>
        </div>
      </div>
      <RouterLink
        to="/"
        class="mr-4 border-1 bg-sky-300 py-1 px-2 rounded-md text-black"
        >Cart <i class="bi bi-cart4 text-xl text-black"></i>
        <span class="rounded-full px-1 py-0 ml-2 bg-sky-700 text-gray-200"
          >29</span
        ></RouterLink
      >
    </div>
    <form class="flex items-center">
      <input
        type="text"
        name="search"
        placeholder="Search for product"
        class="rounded-l-md border-y-2 border-l-2 border-sky-800 bg-gray-50 px-2 text-zinc-600 w-80 search-input"
      />
      <button
        type="submit"
        class="px-2 rounded-r-md border-y-2 border-r-2 border-sky-800 bg-sky-300 text-zinc-600 hover:text-black"
      >
        <i class="bi bi-search"></i> Search
      </button>
    </form>
  </nav>

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
.search-input:focus {
  outline: none !important;
}
.dropdown:hover .dropdown-content {
  display: block;
}
.dropdown-content {
  background-color: #d4f1f4 !important;
  display: none;
}
.ddw-1 {
  width: 600px !important;
}
.ddw-2 {
  width: 225px !important;
}
</style>
