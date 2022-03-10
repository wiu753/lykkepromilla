<template>
  <div>
    <div
      class="h-screen bg-gradient-to-b from-yellow-200 via-yellow-300 to-yellow-500"
    >
      <header class="pt-4 pl-4">
        <LykkepromillaLogo />
      </header>

      <div class="flex items-center h-screen lg:justify-center">
        <div class="flex flex-col mx-5 -mt-32 md:mx-8 lg:mx-12">
          <p class="text-l font-bold md:text-xl lg:text-center">
            Fire lærerstudenter som bare prater sjit.
          </p>
          <h1 class="text-6xl font-bold flex flex-col md:text-7xl md:flex-row">
            <span>LYKKE</span><span class="-mt-10 md:mt-0">PROMILLA</span>
          </h1>
          <div class="flex lg:justify-center">
            <span
              ><a
                href="https://open.spotify.com/show/3HQXcnXX9anhUwD88Z8WPC?si=72a23786e8a942cf"
                ><SpotifySVG class="mr-2" /></a></span
            ><span
              ><a
                href="https://podcasts.apple.com/no/podcast/lykkepromilla/id1609264869"
                ><ApplePodcastSVG /></a
            ></span>
          </div>
        </div>
      </div>
    </div>

    <div class="py-32 px-5 bg-yellow-50 md:py-52 lg:py-56 md:px-8 lg:px-12">
      <p class="italic mb-2 text-xl">Kort historie lang...</p>
      <p class="text-2xl">
        Lykkepromilla er Norges #1 podcast. Vi er på
        <span class="text-orange-800 underline"
          ><a
            href="https://open.spotify.com/show/3HQXcnXX9anhUwD88Z8WPC?si=72a23786e8a942cf"
            class="hover:text-red-700"
            >Spotify</a
          ></span
        >
        og
        <span class="text-orange-800 underline"
          ><a
            href="https://podcasts.apple.com/no/podcast/lykkepromilla/id1609264869"
            class="hover:text-red-700"
            >Apple Podcast</a
          ></span
        >.
      </p>
    </div>
    <footer class="bg-gray-700 items-center flex flex-col pb-20 lg:pb-28">
      <WaveSVG />

      <div class="flex justify-center py-10 lg:py-0 lg:pb-10">
        <a href="https://www.instagram.com/lykkepromilla/"
          ><InstagramSVG class="mr-5"
        /></a>
        <a href="mailto:info@lykkepromilla.no"><EmailSVG /></a>
      </div>
    </footer>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'IndexPage',
})
</script>
