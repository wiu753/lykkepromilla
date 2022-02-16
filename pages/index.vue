<template>
<!-- NEED TO ADD MAIN PART TO A COMPONENT, AND THE STUFF THAT SHOULD LOAD WHEN U CLICK MOBILE BUTTON TO A COMPONENT
THEN LOAD IT LIKE MATT SITE -->
  <div class="flex flex-col">
    <MobileMenu :class="mobileMenu ? 'block' : 'hidden'" />
    <div
      class="h-screen bg-gradient-to-b from-yellow-200 via-yellow-300 to-yellow-500 px-2 pt-2"
    >
      <div class="flex flex-col">
        <header class="flex place-content-between">
          <img
            class="h-14 w-14"
            src="~/assets/lykkepromilla_logo.png"
            alt="Lykkepromilla logo"
          />
          <!-- <div class="flex">
            <img
              class="h-8 w-8 mr-3"
              src="~/assets/instagram.svg"
              alt="Instagram icon"
            />
            <img class="h-8 w-8" src="~/assets/email.svg" alt="Email icon" />
          </div> -->
          <div class="flex items-center py-4 sm:hidden">
            <button
              class="inline-flex items-center justify-center text-gray-400 ease-in-out rounded-md focus:outline-none"
              aria-label="Main menu"
              aria-expanded="false"
              @click="toggleMobileMenu"
            >
              <!-- Icon when menu is closed. -->
              <svg
                v-show="!mobileMenu"
                class="block w-6 h-6"
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
                class="w-6 h-6"
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
        </header>
        <div class="mt-36 text-center">
          <p class="punchline text-l font-bold">
            Fire lærerstudenter som bare prater sjit.
          </p>
          <h1 class="punchline text-6xl font-bold mt-20 flex flex-col">
            <span>LYKKE</span><span class="-mt-10">PROMILLA</span>
          </h1>
          <div><span>Spotify </span><span>Apple</span></div>
        </div>
      </div>
    </div>
    <div>Dette er en podcast om...</div>
    <footer>Footer</footer>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'IndexPage',
  data() {
    return {
      mobileMenu: false
    }
  },
  methods: {
    toggleMobileMenu() {
      this.mobileMenu = !this.mobileMenu
    }
  }
})
</script>
