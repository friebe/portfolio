<script setup lang="ts">
import { useHead } from '@vueuse/head'

// https://github.com/vueuse/head
// you can use this to manipulate the document head in any components,
// they will be renedered correctly in the html results with vite-ssg
useHead({
  meta: [
    { property: 'og:title', content: 'Jan Friebe' },
    { property: 'og:image', content: '' },
    { name: 'description', content: 'Jan Friebe\'s Portfolio' },
    { name: 'twitter:card', content: 'summary' },
    { name: 'twitter:creator', content: '@jan_friebe' },
  ],
})
</script>

<template>
  <NavBar />
  <main class="px-7 py-10">
    <router-view />
    <Footer />
  </main>
</template>
