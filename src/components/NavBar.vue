<script setup>
import { RouterLink } from "vue-router";
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
          class="dropdown-content absolute text-gray-600 py-2 px-4 rounded-md ddw-1 drop-shadow-lg"
        >
          <div class="flex items-center my-2">
            <div class="categories">
              <p class="text-xl text-black">Phones & Phone Accessories</p>
              <div class="flex flex-col ml-2">
                <RouterLink to="/" class="hover:text-black underline"
                  >Tablets</RouterLink
                >
                <RouterLink to="/" class="hover:text-black underline"
                  >Phone Cases</RouterLink
                >
                <RouterLink to="/" class="hover:text-black underline"
                  >Mobile Phones</RouterLink
                >
                <RouterLink to="/" class="hover:text-black underline"
                  >Phone Holders</RouterLink
                >
                <RouterLink to="/" class="hover:text-black underline"
                  >Phone Decoration</RouterLink
                >
                <RouterLink to="/" class="hover:text-black underline"
                  >Screen Protectors</RouterLink
                >
              </div>
            </div>
            <div class="categories">
              <p class="text-xl text-black">Computers & Computer Accessories</p>
              <div class="flex flex-col ml-2">
                <RouterLink to="/" class="hover:text-black underline"
                  >PCs</RouterLink
                >
                <RouterLink to="/" class="hover:text-black underline"
                  >Mini PCs</RouterLink
                >
                <RouterLink to="/" class="hover:text-black underline"
                  >Input Accessories</RouterLink
                >
                <RouterLink to="/" class="hover:text-black underline"
                  >Output Accessories</RouterLink
                >
                <RouterLink to="/" class="hover:text-black underline"
                  >Individual Components</RouterLink
                >
                <RouterLink to="/" class="hover:text-black underline"
                  >Other Computer Accessories</RouterLink
                >
              </div>
            </div>
          </div>
          <div class="flex items-center my-2">
            <div class="categories">
              <p class="text-xl text-black">Commonly Used Accessories</p>
              <div class="flex flex-col ml-2">
                <RouterLink to="/" class="hover:text-black underline"
                  >Cables</RouterLink
                >
                <RouterLink to="/" class="hover:text-black underline"
                  >Memory Cards</RouterLink
                >
                <RouterLink to="/" class="hover:text-black underline"
                  >Stickers & Skins</RouterLink
                >
                <RouterLink to="/" class="hover:text-black underline"
                  >Mounts & Stands</RouterLink
                >
                <RouterLink to="/" class="hover:text-black underline"
                  >Adapters & Connectors</RouterLink
                >
                <RouterLink to="/" class="hover:text-black underline"
                  >Other Commonly Used Accessories</RouterLink
                >
              </div>
            </div>
            <div class="categories">
              <p class="text-xl text-black">Used Electronics</p>
              <div class="flex flex-col ml-2">
                <RouterLink to="/" class="hover:text-black underline"
                  >Used Tablets</RouterLink
                >
                <RouterLink to="/" class="hover:text-black underline"
                  >Used Laptops</RouterLink
                >
                <RouterLink to="/" class="hover:text-black underline"
                  >Used Desktops</RouterLink
                >
                <RouterLink to="/" class="hover:text-black underline"
                  >Used Mobile Phones</RouterLink
                >
                <RouterLink to="/" class="hover:text-black underline"
                  >Used Digital Cameras</RouterLink
                >
                <RouterLink to="/" class="hover:text-black underline"
                  >Other Used Electronics</RouterLink
                >
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="dropdown relative">
        <RouterLink to="/" class="mr-4 hover:text-white"
          >Accounts <i class="bi bi-caret-down-fill text-sm"></i
        ></RouterLink>
        <div
          class="dropdown-content absolute text-gray-600 rounded-md ddw-2 p-2 drop-shadow-lg"
        >
          <RouterLink to="/" class="px-1 my-1 hover:text-black"
            >Saved Items</RouterLink
          >
          <RouterLink to="/" class="px-1 my-1 hover:text-black"
            >Orders History</RouterLink
          >
          <RouterLink to="/" class="px-1 my-1 hover:text-black"
            >Sign in / Sign up</RouterLink
          >
        </div>
      </div>
      <div class="dropdown relative">
        <RouterLink to="/" class="mr-4 hover:text-white"
          >More <i class="bi bi-caret-down-fill text-sm"></i
        ></RouterLink>
        <div
          class="dropdown-content absolute text-gray-600 rounded-md ddw-2 p-2 drop-shadow-lg"
        >
          <RouterLink to="/about" class="px-1 my-1 hover:text-black"
            >About Us</RouterLink
          >
          <RouterLink to="/" class="px-1 my-1 hover:text-black"
            >Contact Us</RouterLink
          >
          <RouterLink to="/" class="px-1 my-1 hover:text-black"
            >Help Center</RouterLink
          >
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
</template>

<script></script>

<style scoped>
.search-input:focus {
  outline: none !important;
}
.dropdown:hover .dropdown-content {
  display: flex;
  flex-direction: column;
}
.dropdown-content {
  background-color: #d4f1f4 !important;
  display: none;
}
.ddw-1 {
  width: 750px !important;
}
.ddw-2 {
  width: 200px !important;
}
.categories {
  width: 50% !important;
}
</style>
