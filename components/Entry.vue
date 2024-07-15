<template>
  <li class="relative marker:text-sky-600 mb-4">
    <div class="flex">
      <div class="grow">
        <h3 class="font-semibold text-lg text-sky-600">{{ position }}</h3>
        <a class="block font-medium" :href="href" target="_blank" rel="noopener">{{ company }}</a>
        <p class="text-gray-700">
          {{ startDate.toLocaleDateString('en-US', { month: 'short', year: 'numeric' }) }}
          &ndash;
          {{ endDate ? endDate.toLocaleDateString('en-US', { month: 'short', year: 'numeric' }) : 'Present' }}
        </p>
      </div>
      <a class="grow-0" :href="href" target="_blank" rel="noopener">
        <NuxtImg class="w-[75px] h-[75px] rounded-lg" :src="imageUrl" :alt="company" />
      </a>
    </div>
    <ul class="list-disc pl-6">
      <li v-for="highlight of highlights" :key="highlight" class="text-gray-600 marker:text-gray-900/75 mt-1.5">
        {{ highlight }}
      </li>
    </ul>
  </li>
</template>

<style scoped>
ul::before {
  content: "";
  display: block;
  position: absolute;
  top: 33px;
  left: -1rem;
  bottom: 5px;
  width: 3px;
  @apply bg-gray-900/10;
}
</style>

<script setup lang="ts">
const props = defineProps<{
  href: string
  position: string
  company: string
  imageUrl?: string
  startDate: Date
  endDate?: Date
  highlights: string[]
}>()
</script>