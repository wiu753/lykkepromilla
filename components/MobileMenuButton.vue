<template>
  <div class="flex items-center py-4 sm:hidden z-40">
    <button
      class="inline-flex items-center justify-center text-black ease-in-out rounded-md focus:outline-none"
      aria-label="Main menu"
      aria-expanded="false"
      @click="toggleMobileMenu"
    >
      <!-- Icon when menu is closed. -->
      <svg
        v-show="!mobileMenu"
        class="block w-8 h-8"
        stroke="currentColor"
        fill="none"
        viewBox="0 0 24 24"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M4 6h16M4 12h16M4 18h16"
        />
      </svg>
      <!-- Icon when menu is open. -->
      <svg
        v-show="mobileMenu"
        class="w-8 h-8"
        stroke="currentColor"
        fill="none"
        viewBox="0 0 24 24"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M6 18L18 6M6 6l12 12"
        />
      </svg>
    </button>
  </div>
</template>
