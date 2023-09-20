<script setup>
import { convertDate } from '../utils'
</script>

<template>
  <NavigationBar />
  <div class="flex justify-center gap-5">
    <main
    class="relative mx-auto max-w-3xl overflow-hidden bg-white py-16 px-2 sm:px-4 lg:px-6"
  >
    <nuxt-link
      class="block cursor-pointer"
      href="/blog"
    >
      <svg
        xmlns="http://www.w3.org/2000/svg"
        class="inline h-6 w-6"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
        stroke-width="2"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          d="M11 17l-5-5m0 0l5-5m-5 5h12"
        />
      </svg>
      Back
    </nuxt-link>
    <ContentDoc v-slot="{ doc }">
      <h2 class="my-4 text-4xl font-semibold">{{ doc.title }}</h2>
      <p class="my-4 text-gray-500">
        by, {{ doc.author }}, {{ convertDate(doc.date) }}
      </p>
      <div
        class="prose prose-lg first-letter:text-3xl first-letter:text-blue-600"
      >
        <ContentRenderer :value="doc" />
      </div>
    </ContentDoc>
  </main>
    <div class="min-h-screen w-80 border-l-2 border-gray-300 relative">

        <div class="sticky top-10 mt-20 p-5 mx-auto w-fit">
          <div class="flex flex-col">
            <div class="font-bold">Contents</div>
          </div>
      </div>
    </div>
  </div>
</template>
