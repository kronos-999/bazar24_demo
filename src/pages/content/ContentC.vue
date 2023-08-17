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
      <div class="mb-20 w-full flex flex-col flex-wrap items-center text-center">
        <h1 class="title-font mb-2 text-2xl font-medium text-gray-900 sm:text-3xl dark:text-white">
          Pitchfork Kickstarter Taxidermy
        </h1>
        <p class="w-full leading-relaxed text-gray-500 lg:w-1/2 dark:text-opacity-80">
          Whatever cardigan tote bag tumblr hexagon brooklyn asymmetrical gentrify, subway tile poke farm-to-table.
        </p>
      </div>
      <div class="flex flex-wrap -m-4">
        <div class="p-4 md:w-1/2 xl:w-1/3">
          <div class="border border-gray-200 rounded-lg p-6 dark:border-gray-700 dark:border-opacity-75">
            <div
              :class="`w-10 h-10 inline-flex items-center justify-center rounded-full bg-${theme}-100 text-${theme}-500 mb-4 dark:bg-gray-800 dark:text-${theme}-400`"
            >
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                class="h-6 w-6" viewBox="0 0 24 24"
              >
                <path d="M22 12h-4l-3 9L9 3l-3 9H2" />
              </svg>
            </div>
            <h2 class="title-font mb-2 text-lg font-medium text-gray-900 dark:text-white">
              Shooting Stars
            </h2>
            <p class="text-base leading-relaxed">
              Fingerstache flexitarian street art 8-bit waist co, subway tile poke farm.
            </p>
          </div>
        </div>
        <div class="p-4 md:w-1/2 xl:w-1/3">
          <div class="border border-gray-200 rounded-lg p-6 dark:border-gray-700 dark:border-opacity-75">
            <div
              :class="`w-10 h-10 inline-flex items-center justify-center rounded-full bg-${theme}-100 text-${theme}-500 mb-4 dark:bg-gray-800 dark:text-${theme}-400`"
            >
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                class="h-6 w-6" viewBox="0 0 24 24"
              >
                <circle cx="6" cy="6" r="3" />
                <circle cx="6" cy="18" r="3" />
                <path d="M20 4L8.12 15.88M14.47 14.48L20 20M8.12 8.12L12 12" />
              </svg>
            </div>
            <h2 class="title-font mb-2 text-lg font-medium text-gray-900 dark:text-white">
              The Catalyzer
            </h2>
            <p class="text-base leading-relaxed">
              Fingerstache flexitarian street art 8-bit waist co, subway tile poke farm.
            </p>
          </div>
        </div>
        <div class="p-4 md:w-1/2 xl:w-1/3">
          <div class="border border-gray-200 rounded-lg p-6 dark:border-gray-700 dark:border-opacity-75">
            <div
              :class="`w-10 h-10 inline-flex items-center justify-center rounded-full bg-${theme}-100 text-${theme}-500 mb-4 dark:bg-gray-800 dark:text-${theme}-400`"
            >
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                class="h-6 w-6" viewBox="0 0 24 24"
              >
                <path d="M20 21v-2a4 4 0 00-4-4H8a4 4 0 00-4 4v2" />
                <circle cx="12" cy="7" r="4" />
              </svg>
            </div>
            <h2 class="title-font mb-2 text-lg font-medium text-gray-900 dark:text-white">
              Neptune
            </h2>
            <p class="text-base leading-relaxed">
              Fingerstache flexitarian street art 8-bit waist co, subway tile poke farm.
            </p>
          </div>
        </div>
        <div class="p-4 md:w-1/2 xl:w-1/3">
          <div class="border border-gray-200 rounded-lg p-6 dark:border-gray-700 dark:border-opacity-75">
            <div
              :class="`w-10 h-10 inline-flex items-center justify-center rounded-full bg-${theme}-100 text-${theme}-500 mb-4 dark:bg-gray-800 dark:text-${theme}-400`"
            >
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                class="h-6 w-6" viewBox="0 0 24 24"
              >
                <path d="M4 15s1-1 4-1 5 2 8 2 4-1 4-1V3s-1 1-4 1-5-2-8-2-4 1-4 1zM4 22v-7" />
              </svg>
            </div>
            <h2 class="title-font mb-2 text-lg font-medium text-gray-900 dark:text-white">
              Melanchole
            </h2>
            <p class="text-base leading-relaxed">
              Fingerstache flexitarian street art 8-bit waist co, subway tile poke farm.
            </p>
          </div>
        </div>
        <div class="p-4 md:w-1/2 xl:w-1/3">
          <div class="border border-gray-200 rounded-lg p-6 dark:border-gray-700 dark:border-opacity-75">
            <div
              :class="`w-10 h-10 inline-flex items-center justify-center rounded-full bg-${theme}-100 text-${theme}-500 mb-4 dark:bg-gray-800 dark:text-${theme}-400`"
            >
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                class="h-6 w-6" viewBox="0 0 24 24"
              >
                <path d="M21 12.79A9 9 0 1111.21 3 7 7 0 0021 12.79z" />
              </svg>
            </div>
            <h2 class="title-font mb-2 text-lg font-medium text-gray-900 dark:text-white">
              Bunker
            </h2>
            <p class="text-base leading-relaxed">
              Fingerstache flexitarian street art 8-bit waist co, subway tile poke farm.
            </p>
          </div>
        </div>
        <div class="p-4 md:w-1/2 xl:w-1/3">
          <div class="border border-gray-200 rounded-lg p-6 dark:border-gray-700 dark:border-opacity-75">
            <div
              :class="`w-10 h-10 inline-flex items-center justify-center rounded-full bg-${theme}-100 text-${theme}-500 mb-4 dark:bg-gray-800 dark:text-${theme}-400`"
            >
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                class="h-6 w-6" viewBox="0 0 24 24"
              >
                <path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z" />
              </svg>
            </div>
            <h2 class="title-font mb-2 text-lg font-medium text-gray-900 dark:text-white">
              Ramona Falls
            </h2>
            <p class="text-base leading-relaxed">
              Fingerstache flexitarian street art 8-bit waist co, subway tile poke farm.
            </p>
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
