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
    <div class="mx-auto flex flex-wrap px-5 py-24 container">
      <div class="relative mx-auto flex pb-20 pt-10 md:w-2/3 sm:items-center">
        <div class="absolute inset-0 h-full w-6 flex items-center justify-center">
          <div class="pointer-events-none h-full w-1 bg-gray-200 dark:bg-gray-800" />
        </div>
        <div
          :class="`flex-shrink-0 w-6 h-6 rounded-full mt-10 sm:mt-0 inline-flex items-center justify-center bg-${theme}-500 text-white relative z-10 title-font font-medium text-sm`"
        >
          1
        </div>
        <div class="flex flex-grow flex-col items-start pl-6 sm:flex-row sm:items-center md:pl-8">
          <div
            :class="`flex-shrink-0 w-24 h-24 bg-${theme}-100 text-${theme}-500 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
          >
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              class="h-12 w-12" viewBox="0 0 24 24"
            >
              <path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z" />
            </svg>
          </div>
          <div class="mt-6 flex-grow sm:mt-0 sm:pl-6">
            <h2 class="title-font mb-1 text-xl font-medium text-gray-900 dark:text-white">
              Shooting Stars
            </h2>
            <p class="leading-relaxed">
              VHS cornhole pop-up, try-hard 8-bit iceland helvetica. Kinfolk bespoke try-hard cliche palo santo offal.
            </p>
          </div>
        </div>
      </div>
      <div class="relative mx-auto flex pb-20 md:w-2/3 sm:items-center">
        <div class="absolute inset-0 h-full w-6 flex items-center justify-center">
          <div class="pointer-events-none h-full w-1 bg-gray-200 dark:bg-gray-800" />
        </div>
        <div
          :class="`flex-shrink-0 w-6 h-6 rounded-full mt-10 sm:mt-0 inline-flex items-center justify-center bg-${theme}-500 text-white relative z-10 title-font font-medium text-sm`"
        >
          2
        </div>
        <div class="flex flex-grow flex-col items-start pl-6 sm:flex-row sm:items-center md:pl-8">
          <div
            :class="`flex-shrink-0 w-24 h-24 bg-${theme}-100 text-${theme}-500 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
          >
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              class="h-12 w-12" viewBox="0 0 24 24"
            >
              <path d="M22 12h-4l-3 9L9 3l-3 9H2" />
            </svg>
          </div>
          <div class="mt-6 flex-grow sm:mt-0 sm:pl-6">
            <h2 class="title-font mb-1 text-xl font-medium text-gray-900 dark:text-white">
              The Catalyzer
            </h2>
            <p class="leading-relaxed">
              VHS cornhole pop-up, try-hard 8-bit iceland helvetica. Kinfolk bespoke try-hard cliche palo santo offal.
            </p>
          </div>
        </div>
      </div>
      <div class="relative mx-auto flex pb-20 md:w-2/3 sm:items-center">
        <div class="absolute inset-0 h-full w-6 flex items-center justify-center">
          <div class="pointer-events-none h-full w-1 bg-gray-200 dark:bg-gray-800" />
        </div>
        <div
          :class="`flex-shrink-0 w-6 h-6 rounded-full mt-10 sm:mt-0 inline-flex items-center justify-center bg-${theme}-500 text-white relative z-10 title-font font-medium text-sm`"
        >
          3
        </div>
        <div class="flex flex-grow flex-col items-start pl-6 sm:flex-row sm:items-center md:pl-8">
          <div
            :class="`flex-shrink-0 w-24 h-24 bg-${theme}-100 text-${theme}-500 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
          >
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              class="h-12 w-12" viewBox="0 0 24 24"
            >
              <circle cx="12" cy="5" r="3" />
              <path d="M12 22V8M5 12H2a10 10 0 0020 0h-3" />
            </svg>
          </div>
          <div class="mt-6 flex-grow sm:mt-0 sm:pl-6">
            <h2 class="title-font mb-1 text-xl font-medium text-gray-900 dark:text-white">
              The 400 Blows
            </h2>
            <p class="leading-relaxed">
              VHS cornhole pop-up, try-hard 8-bit iceland helvetica. Kinfolk bespoke try-hard cliche palo santo offal.
            </p>
          </div>
        </div>
      </div>
      <div class="relative mx-auto flex pb-10 md:w-2/3 sm:items-center">
        <div class="absolute inset-0 h-full w-6 flex items-center justify-center">
          <div class="pointer-events-none h-full w-1 bg-gray-200 dark:bg-gray-800" />
        </div>
        <div
          :class="`flex-shrink-0 w-6 h-6 rounded-full mt-10 sm:mt-0 inline-flex items-center justify-center bg-${theme}-500 text-white relative z-10 title-font font-medium text-sm`"
        >
          4
        </div>
        <div class="flex flex-grow flex-col items-start pl-6 sm:flex-row sm:items-center md:pl-8">
          <div
            :class="`flex-shrink-0 w-24 h-24 bg-${theme}-100 text-${theme}-500 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
          >
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              class="h-12 w-12" viewBox="0 0 24 24"
            >
              <path d="M20 21v-2a4 4 0 00-4-4H8a4 4 0 00-4 4v2" />
              <circle cx="12" cy="7" r="4" />
            </svg>
          </div>
          <div class="mt-6 flex-grow sm:mt-0 sm:pl-6">
            <h2 class="title-font mb-1 text-xl font-medium text-gray-900 dark:text-white">
              Neptune
            </h2>
            <p class="leading-relaxed">
              VHS cornhole pop-up, try-hard 8-bit iceland helvetica. Kinfolk bespoke try-hard cliche palo santo offal.
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>

<style></style>
