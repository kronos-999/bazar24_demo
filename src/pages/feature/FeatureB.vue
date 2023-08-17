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
        <h1 class="title-font mb-4 text-2xl font-medium text-gray-900 sm:text-3xl dark:text-white">
          Raw Denim Heirloom Man Braid
        </h1>
        <p
          class="text-gray-500s mx-auto text-base leading-relaxed lg:w-3/4 xl:w-2/4 dark:text-gray-400 dark:text-opacity-80"
        >
          Blue bottle crucifix vinyl post-ironic four dollar toast vegan taxidermy. Gastropub indxgo juice poutine,
          ramps microdosing banh mi pug.
        </p>
        <div class="mt-6 flex justify-center">
          <div :class="`w-16 h-1 rounded-full bg-${theme}-500 inline-flex`" />
        </div>
      </div>
      <div class="flex flex-wrap -mx-4 -mb-10 -mt-4 space-y-6 sm:-m-4 md:space-y-0">
        <div class="flex flex-col items-center p-4 text-center md:w-1/3">
          <div
            :class="`w-20 h-20 inline-flex items-center justify-center rounded-full bg-${theme}-100 text-${theme}-500 mb-5 flex-shrink-0 dark:bg-gray-800 dark:text-${theme}-400`"
          >
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              class="h-10 w-10" viewBox="0 0 24 24"
            >
              <path d="M22 12h-4l-3 9L9 3l-3 9H2" />
            </svg>
          </div>
          <div class="flex-grow">
            <h2 class="title-font mb-3 text-lg font-medium text-gray-900 dark:text-white">
              Shooting Stars
            </h2>
            <p class="text-base leading-relaxed">
              Blue bottle crucifix vinyl post-ironic four dollar toast vegan taxidermy. Gastropub indxgo juice poutine,
              ramps microdosing banh mi pug VHS try-hard.
            </p>
            <a :class="`mt-3 text-${theme}-500 inline-flex items-center dark:text-${theme}-400`">Learn More
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                class="ml-2 h-4 w-4" viewBox="0 0 24 24"
              >
                <path d="M5 12h14M12 5l7 7-7 7" />
              </svg>
            </a>
          </div>
        </div>
        <div class="flex flex-col items-center p-4 text-center md:w-1/3">
          <div
            :class="`w-20 h-20 inline-flex items-center justify-center rounded-full bg-${theme}-100 text-${theme}-500 mb-5 flex-shrink-0 dark:bg-gray-800 dark:text-${theme}-400`"
          >
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              class="h-10 w-10" viewBox="0 0 24 24"
            >
              <circle cx="6" cy="6" r="3" />
              <circle cx="6" cy="18" r="3" />
              <path d="M20 4L8.12 15.88M14.47 14.48L20 20M8.12 8.12L12 12" />
            </svg>
          </div>
          <div class="flex-grow">
            <h2 class="title-font mb-3 text-lg font-medium text-gray-900 dark:text-white">
              The Catalyzer
            </h2>
            <p class="text-base leading-relaxed">
              Blue bottle crucifix vinyl post-ironic four dollar toast vegan taxidermy. Gastropub indxgo juice poutine,
              ramps microdosing banh mi pug VHS try-hard.
            </p>
            <a :class="`mt-3 text-${theme}-500 inline-flex items-center dark:text-${theme}-400`">Learn More
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                class="ml-2 h-4 w-4" viewBox="0 0 24 24"
              >
                <path d="M5 12h14M12 5l7 7-7 7" />
              </svg>
            </a>
          </div>
        </div>
        <div class="flex flex-col items-center p-4 text-center md:w-1/3">
          <div
            :class="`w-20 h-20 inline-flex items-center justify-center rounded-full bg-${theme}-100 text-${theme}-500 mb-5 flex-shrink-0 dark:bg-gray-800 dark:text-${theme}-400`"
          >
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              class="h-10 w-10" viewBox="0 0 24 24"
            >
              <path d="M20 21v-2a4 4 0 00-4-4H8a4 4 0 00-4 4v2" />
              <circle cx="12" cy="7" r="4" />
            </svg>
          </div>
          <div class="flex-grow">
            <h2 class="title-font mb-3 text-lg font-medium text-gray-900 dark:text-white">
              Neptune
            </h2>
            <p class="text-base leading-relaxed">
              Blue bottle crucifix vinyl post-ironic four dollar toast vegan taxidermy. Gastropub indxgo juice poutine,
              ramps microdosing banh mi pug VHS try-hard.
            </p>
            <a :class="`mt-3 text-${theme}-500 inline-flex items-center dark:text-${theme}-400`">Learn More
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                class="ml-2 h-4 w-4" viewBox="0 0 24 24"
              >
                <path d="M5 12h14M12 5l7 7-7 7" />
              </svg>
            </a>
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
