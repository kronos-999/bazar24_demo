<script>
export default {
  props: {
    theme: {
      type: String,
      default: 'red',
    },
  },
}
</script>

<template>
  <section class="body-font text-gray-600 dark:bg-gray-900 dark:text-gray-400">
    <div class="mx-auto px-5 py-24 container">
      <div class="mb-20 text-center">
        <h1 class="title-font mb-4 text-center text-2xl font-medium text-gray-900 sm:text-3xl dark:text-white">
          Raw Denim Heirloom Man Braid
        </h1>
        <p class="mx-auto text-base leading-relaxed lg:w-3/4 xl:w-2/4">
          Blue bottle crucifix vinyl post-ironic four dollar toast vegan taxidermy. Gastropub indxgo juice poutine,
          ramps microdosing banh mi pug.
        </p>
      </div>
      <div class="flex flex-wrap -mx-2 sm:mx-auto sm:mb-2 lg:w-4/5">
        <div class="w-full p-2 sm:w-1/2">
          <div class="h-full flex items-center rounded bg-gray-100 p-4 dark:bg-gray-800">
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
              :class="`text-${theme}-500 w-6 h-6 flex-shrink-0 mr-4 dark:text-${theme}-400`" viewBox="0 0 24 24"
            >
              <path d="M22 11.08V12a10 10 0 11-5.93-9.14" />
              <path d="M22 4L12 14.01l-3-3" />
            </svg>
            <span class="title-font font-medium dark:text-white">Authentic Cliche Forage</span>
          </div>
        </div>
        <div class="w-full p-2 sm:w-1/2">
          <div class="h-full flex items-center rounded bg-gray-100 p-4 dark:bg-gray-800">
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
              :class="`text-${theme}-500 w-6 h-6 flex-shrink-0 mr-4 dark:text-${theme}-400`" viewBox="0 0 24 24"
            >
              <path d="M22 11.08V12a10 10 0 11-5.93-9.14" />
              <path d="M22 4L12 14.01l-3-3" />
            </svg>
            <span class="title-font font-medium dark:text-white">Kinfolk Chips Snackwave</span>
          </div>
        </div>
        <div class="w-full p-2 sm:w-1/2">
          <div class="h-full flex items-center rounded bg-gray-100 p-4 dark:bg-gray-800">
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
              :class="`text-${theme}-500 w-6 h-6 flex-shrink-0 mr-4 dark:text-${theme}-400`" viewBox="0 0 24 24"
            >
              <path d="M22 11.08V12a10 10 0 11-5.93-9.14" />
              <path d="M22 4L12 14.01l-3-3" />
            </svg>
            <span class="title-font font-medium dark:text-white">Coloring Book Ethical</span>
          </div>
        </div>
        <div class="w-full p-2 sm:w-1/2">
          <div class="h-full flex items-center rounded bg-gray-100 p-4 dark:bg-gray-800">
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
              :class="`text-${theme}-500 w-6 h-6 flex-shrink-0 mr-4 dark:text-${theme}-400`" viewBox="0 0 24 24"
            >
              <path d="M22 11.08V12a10 10 0 11-5.93-9.14" />
              <path d="M22 4L12 14.01l-3-3" />
            </svg>
            <span class="title-font font-medium dark:text-white">Typewriter Polaroid Cray</span>
          </div>
        </div>
        <div class="w-full p-2 sm:w-1/2">
          <div class="h-full flex items-center rounded bg-gray-100 p-4 dark:bg-gray-800">
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
              :class="`text-${theme}-500 w-6 h-6 flex-shrink-0 mr-4 dark:text-${theme}-400`" viewBox="0 0 24 24"
            >
              <path d="M22 11.08V12a10 10 0 11-5.93-9.14" />
              <path d="M22 4L12 14.01l-3-3" />
            </svg>
            <span class="title-font font-medium dark:text-white">Pack Truffaut Blue</span>
          </div>
        </div>
        <div class="w-full p-2 sm:w-1/2">
          <div class="h-full flex items-center rounded bg-gray-100 p-4 dark:bg-gray-800">
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
              :class="`text-${theme}-500 w-6 h-6 flex-shrink-0 mr-4 dark:text-${theme}-400`" viewBox="0 0 24 24"
            >
              <path d="M22 11.08V12a10 10 0 11-5.93-9.14" />
              <path d="M22 4L12 14.01l-3-3" />
            </svg>
            <span class="title-font font-medium dark:text-white">The Catcher In The Rye</span>
          </div>
        </div>
      </div>
      <button
        :class="`flex mx-auto mt-16 text-white bg-${theme}-500 border-0 py-2 px-8 focus:outline-none hover:bg-${theme}-600 rounded text-lg`"
      >
        Button
      </button>
    </div>
  </section>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>

<style></style>
