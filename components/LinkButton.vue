<template>
  <a :href="href" target="_blank" rel="noopener" class="inline-flex items-center px-4 py-2 rounded-md text-sky-600 text-sm bg-sky-600/10 hover:bg-sky-600/15 transition"><slot /></a>
</template>

<style scoped>
:deep(svg) {
  @apply h-3.5 w-3.5 ml-1.5;
}
</style>

<script setup lang="ts">
const props = defineProps<{href: string}>()
</script>
