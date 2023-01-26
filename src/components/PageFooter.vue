<script setup>
import { RouterLink } from "vue-router";
</script>

<template>
  <footer class="py-4 bg-sky-700 text-gray-200">
    <div class="flex flex-row px-32 my-4">
      <div>
        <p class="text-xl font-bold">Let's Help You</p>
        <div class="flex flex-col">
          <RouterLink to="/" class="hover:text-white">Help center</RouterLink>
          <RouterLink to="/" class="hover:text-white"
            >Shipping and delivery</RouterLink
          >
          <RouterLink to="/" class="hover:text-white">Return policy</RouterLink>
          <RouterLink to="/" class="hover:text-white"
            >Report an item</RouterLink
          >
        </div>
      </div>
      <div class="ml-16">
        <p class="text-xl font-bold">Make Money With Us</p>
        <div class="flex flex-col">
          <RouterLink to="/" class="hover:text-white"
            >Sell on Gadget Shop</RouterLink
          >
          <RouterLink to="/" class="hover:text-white"
            >Become a logistics service provider</RouterLink
          >
          <RouterLink to="/" class="hover:text-white"
            >Become a products supplier</RouterLink
          >
        </div>
      </div>
      <div class="ml-16">
        <p class="text-xl font-bold">Coming soon</p>
        <p><i class="bi bi-apple text-2xl"></i> iOS app</p>
        <p><i class="bi bi-android2 text-2xl"></i> Android app</p>
      </div>
      <form class="ml-16">
        <p class="text-xl font-bold">Subscribe to our newsletter</p>
        <div>
          <input
            type="text"
            name="search"
            placeholder="Your email address"
            class="rounded-l-md border-y-2 border-l-2 border-sky-800 bg-gray-50 px-2 text-zinc-600 w-60 search-input"
          />
          <button
            type="submit"
            class="px-2 rounded-r-md border-y-2 border-r-2 border-sky-800 bg-sky-300 text-zinc-600 hover:text-black"
          >
            <i class="bi bi-newspaper"></i> Subscribe
          </button>
        </div>
      </form>
    </div>
    <div class="flex flex-row bg-sky-900 px-32 py-4">
      <p>
        <i class="bi bi-c-circle"></i> 2023
        <span class="font-semibold">Gadget Shop</span>
      </p>
      <RouterLink to="/" class="ml-16 underline">Terms of use</RouterLink>
      <RouterLink to="/" class="ml-16 underline">Privacy</RouterLink>
    </div>
  </footer>
</template>

<script></script>

<style scoped></style>
