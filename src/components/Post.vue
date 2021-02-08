<template>
  <div v-if="frontmatter.display || frontmatter.title" class="prose m-auto mb-8">
    <h1 class="mb-0">
      {{ frontmatter.display || frontmatter.title }}
    </h1>
  </div>
  <slot />
</template>

<script setup lang="ts">
import { defineProps, onMounted } from 'vue'
const { frontmatter } = defineProps<{ frontmatter: any }>()

</script>
