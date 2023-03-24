<template>
  <div class="bg-gradient-to-l from-yellow-500 via-purple-500 to-blue-500">
    <nav class="container px-6 py-8 mx-auto md:flex md:justify-between md:items-center">
      <div class="flex items-center justify-between">
        <router-link to="/" class="text-xl font-bold text-gray-100 md:text-2xl hover:text-indigo-400">
          <div class="flex-shrink-0">
            <a href="#" title="" class="flex">
              <img class="w-auto h-8" src="https://cdn.rareblocks.xyz/collection/celebration/images/logo.svg" alt="" />
            </a>
          </div>
        </router-link>
        <!-- Mobile menu button -->
        <div @click="toggleNav" class="flex md:hidden">
          <button type="button" class="text-gray-100 hover:text-gray-400 focus:outline-none focus:text-gray-400">
            <svg viewBox="0 0 24 24" class="w-6 h-6 fill-current">
              <path fill-rule="evenodd"
                d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z">
              </path>
            </svg>
          </button>
        </div>
      </div>

      <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
      <ul :class="showMenu ? 'flex' : 'hidden'"
        class="flex-col mt-8 space-y-4 md:flex md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0">
        <li>
          <nuxt-link to="/" class="text-gray-100 hover:text-gray-900">
            Home</nuxt-link>
        </li>
        <li>
          <nuxt-link to="About" class="text-gray-100 hover:text-gray-900">About</nuxt-link>
        </li>
        <li>
          <nuxt-link to="About" class="text-gray-100 hover:text-gray-900">Blogs</nuxt-link>
        </li>
        <li>
          <nuxt-link to="About" class="text-gray-100 hover:text-gray-900">
            Contact Us
          </nuxt-link>
        </li>
      </ul>
      <NuxtLink to="Signup"
        class="relative inline-flex items-center justify-start px-5 py-3 overflow-hidden font-bold rounded-full group">
        <span
          class="w-32 h-32 rotate-45 translate-x-12 -translate-y-2 absolute left-0 top-0 bg-gray-500 opacity-[3%]"></span>
        <span
          class="absolute top-0 left-0 w-48 h-48 -mt-1 transition-all duration-500 ease-in-out rotate-45 -translate-x-56 -translate-y-24 bg-black hover:text-bg-white opacity-100 group-hover:-translate-x-8"></span>
        <span
          class="relative w-full text-left hover:text-white transition-colors duration-200 ease-in-out group-hover:text-white">Sign
          Up</span>
        <span class="absolute inset-0 border-2 border-black rounded-full"></span>
      </NuxtLink>
    </nav>
  </div>
</template>S
<script>
import { ref } from "vue";
export default {
  setup() {
    let showMenu = ref(false);
    const toggleNav = () => (showMenu.value = !showMenu.value);
    return { showMenu, toggleNav };
  },
};
</script>

<style scoped>
@media (max-width: 640px) {
  .relative {
    display: none;
  }
}

@media (max-width: 750px) {
  .relative {
    display: none;
  }
}
</style>



