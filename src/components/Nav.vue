<template>
    <!-- This example requires Tailwind CSS v2.0+ -->
<nav class="bg-white shadow">
  <div class="max-w-7xl mx-auto px-2 sm:px-6 lg:px-8">
    <div class="relative flex justify-between h-16">
      <div class="absolute inset-y-0 right-0 flex items-center sm:hidden">
        <!-- Mobile menu button -->
        <button @click="toggleMenu" type="button" class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-indigo-500" aria-controls="mobile-menu" aria-expanded="false">
          <span class="sr-only">Open main menu</span>
          <!--
            Icon when menu is closed.

            Heroicon name: outline/menu

            Menu open: "hidden", Menu closed: "block"
          -->
          <svg class="block h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
          </svg>
          <!--
            Icon when menu is open.

            Heroicon name: outline/x

            Menu open: "block", Menu closed: "hidden"
          -->
          <svg class="hidden h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
          </svg>
        </button>
      </div>
      <div class="flex-1 flex sm:items-center lg:items-left lg:justify-left sm:items-stretch sm:justify-center">
        <div class="flex-shrink-0 flex items-left">
          <img class="block lg:hidden h-12 w-auto justify-center" src="../assets/logo.svg" alt="Workflow">
          <img class="hidden lg:block h-14 w-auto justify-items-start" src="../assets/logo.svg" alt="Workflow">
        </div>
      </div>
      <div class="flex-1 flex items-center justify-center sm:items-stretch sm:justify-center">
        <div class="hidden sm:ml-6 sm:flex sm:space-x-14">
          <!-- Current: "border-indigo-500 text-gray-900", Default: "border-transparent text-gray-500 hover:border-gray-300 hover:text-gray-700" -->
          <a href="#team" class="border-transparent text-gray-500 hover:border-black hover:text-black inline-flex items-center px-1 pt-1 border-b-2 text-sm font-bold font-sans"> Team </a>
          <a href="#sponsors" class="border-transparent text-gray-500 hover:border-black hover:text-black inline-flex items-center px-1 pt-1 border-b-2 text-sm font-bold font-sans"> Sponsors </a>
          <a href="#calendar" class="border-transparent text-gray-500 hover:border-black hover:text-black inline-flex items-center px-1 pt-1 border-b-2 text-sm font-bold font-sans"> Calendar </a>
        </div>
      </div>
      <div class="flex-1 flex sm:items-center lg:items-left lg:justify-left sm:items-stretch sm:justify-center">
        <div class="hidden lg:flex-shrink-0 lg:flex lg:items-left">
          <a href="https://www.instagram.com/explore/tags/thanksdart/" target="_blank" class="text-center text-gray-500 block pl-3 pr-4 py-6 text-base font-bold font-sans">#thanksdart</a>
        </div>
      </div>
    </div>
  </div>

  <!-- Mobile menu, show/hide based on menu state. -->
  <div class="sm:hidden" id="mobile-menu" v-if="showMenu">
    <div class="pt-2 pb-4 space-y-1">
      <!-- Current: "bg-indigo-50 border-indigo-500 text-indigo-700", Default: "border-transparent text-gray-500 hover:bg-gray-50 hover:border-gray-300 hover:text-gray-700" -->
      <a href="#team" class="border-transparent text-center text-gray-500 hover:bg-black hover:border-black hover:text-white block pl-3 pr-4 py-2 border-l-4 text-base font-bold font-sans">Team</a>
      <a href="#sponsors" class="border-transparent text-center text-gray-500 hover:bg-black hover:border-black hover:text-white block pl-3 pr-4 py-2 border-l-4 text-base font-bold font-sans">Projects</a>
      <a href="#calendar" class="border-transparent text-center text-gray-500 hover:bg-black hover:border-black hover:text-white block pl-3 pr-4 py-2 border-l-4 text-base font-bold font-sans">Calendar</a>
      <a href="https://www.instagram.com/explore/tags/thanksdart/" target="_blank" class="text-center text-gray-500 hover:bg-black hover:border-black hover:text-white block pl-3 pr-4 py-6 text-base font-bold font-sans">#thanksdart</a>
    </div>
  </div>
</nav>
</template>
<script>
  export default {
    data() {
      return {
        showMenu: false,
      }
    },

    methods: {
      toggleMenu() {
        return this.showMenu = !this.showMenu;
      }
    }
  }
</script>