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
      <h1 class="title-font mb-20 text-center text-2xl font-medium text-gray-900 sm:text-3xl dark:text-white">
        Raw Denim Heirloom Man Braid <br class="hidden sm:block">Selfies Wayfarers
      </h1>
      <div class="flex flex-wrap -mx-4 -mb-10 -mt-4 space-y-6 sm:-m-4 md:space-y-0">
        <div class="flex p-4 md:w-1/3">
          <div
            :class="`w-12 h-12 inline-flex items-center justify-center rounded-full bg-${theme}-100 text-${theme}-500 mb-4 flex-shrink-0 dark:bg-gray-800 dark:text-${theme}-400`"
          >
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              class="h-6 w-6" viewBox="0 0 24 24"
            >
              <path d="M22 12h-4l-3 9L9 3l-3 9H2" />
            </svg>
          </div>
          <div class="flex-grow pl-6">
            <h2 class="title-font mb-2 text-lg font-medium text-gray-900 dark:text-white">
              Shooting Stars
            </h2>
            <p class="text-base leading-relaxed">
              Blue bottle crucifix vinyl post-ironic four dollar toast vegan taxidermy. Gastropub indxgo juice poutine,
              ramps microdosing banh mi pug VHS try-hard ugh iceland kickstarter tumblr live-edge tilde.
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
        <div class="flex p-4 md:w-1/3">
          <div
            :class="`w-12 h-12 inline-flex items-center justify-center rounded-full bg-${theme}-100 text-${theme}-500 mb-4 flex-shrink-0 dark:bg-gray-800 dark:text-${theme}-400`"
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
          <div class="flex-grow pl-6">
            <h2 class="title-font mb-2 text-lg font-medium text-gray-900 dark:text-white">
              The Catalyzer
            </h2>
            <p class="text-base leading-relaxed">
              Blue bottle crucifix vinyl post-ironic four dollar toast vegan taxidermy. Gastropub indxgo juice poutine,
              ramps microdosing banh mi pug VHS try-hard ugh iceland kickstarter tumblr live-edge tilde.
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
        <div class="flex p-4 md:w-1/3">
          <div
            :class="`w-12 h-12 inline-flex items-center justify-center rounded-full bg-${theme}-100 text-${theme}-500 mb-4 flex-shrink-0 dark:bg-gray-800 dark:text-${theme}-400`"
          >
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              class="h-6 w-6" viewBox="0 0 24 24"
            >
              <path d="M20 21v-2a4 4 0 00-4-4H8a4 4 0 00-4 4v2" />
              <circle cx="12" cy="7" r="4" />
            </svg>
          </div>
          <div class="flex-grow pl-6">
            <h2 class="title-font mb-2 text-lg font-medium text-gray-900 dark:text-white">
              Neptune
            </h2>
            <p class="text-base leading-relaxed">
              Blue bottle crucifix vinyl post-ironic four dollar toast vegan taxidermy. Gastropub indxgo juice poutine,
              ramps microdosing banh mi pug VHS try-hard ugh iceland kickstarter tumblr live-edge tilde.
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
    </div>
  </section>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>

<style></style>
