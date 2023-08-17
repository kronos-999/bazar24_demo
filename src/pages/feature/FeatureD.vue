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
      <div class="flex flex-wrap -m-4">
        <div class="p-4 lg:w-1/2 md:w-full">
          <div
            class="flex flex-col border-2 border-gray-200 border-opacity-50 rounded-lg p-8 sm:flex-row dark:border-gray-800"
          >
            <div
              :class="`w-16 h-16 sm:mr-8 sm:mb-0 mb-4 inline-flex items-center justify-center rounded-full bg-${theme}-100 text-${theme}-500 flex-shrink-0 dark:bg-gray-800 dark:text-${theme}-400`"
            >
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                class="h-8 w-8" viewBox="0 0 24 24"
              >
                <path d="M22 12h-4l-3 9L9 3l-3 9H2" />
              </svg>
            </div>
            <div class="flex-grow">
              <h2 class="title-font mb-3 text-lg font-medium text-gray-900 dark:text-white">
                Shooting Stars
              </h2>
              <p class="text-base leading-relaxed">
                Blue bottle crucifix vinyl post-ironic four dollar toast vegan taxidermy. Gastropub indxgo juice
                poutine.
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
        <div class="p-4 lg:w-1/2 md:w-full">
          <div
            class="flex flex-col border-2 border-gray-200 border-opacity-50 rounded-lg p-8 sm:flex-row dark:border-gray-800"
          >
            <div
              :class="`w-16 h-16 sm:mr-8 sm:mb-0 mb-4 inline-flex items-center justify-center rounded-full bg-${theme}-100 text-${theme}-500 flex-shrink-0 dark:bg-gray-800 dark:text-${theme}-400`"
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
                The Catalyzer
              </h2>
              <p class="text-base leading-relaxed">
                Blue bottle crucifix vinyl post-ironic four dollar toast vegan taxidermy. Gastropub indxgo juice
                poutine.
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
    </div>
  </section>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>

<style></style>
