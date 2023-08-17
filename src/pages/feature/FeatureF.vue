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
      <div
        class="mx-auto mb-10 flex flex-col items-center border-b border-gray-200 pb-10 lg:w-3/5 sm:flex-row dark:border-gray-800"
      >
        <div
          :class="`sm:w-32 sm:h-32 h-20 w-20 sm:mr-10 inline-flex items-center justify-center rounded-full bg-${theme}-100 text-${theme}-500 flex-shrink-0 dark:text-${theme}-400 dark:bg-gray-800`"
        >
          <svg
            fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
            class="h-10 w-10 sm:h-16 sm:w-16" viewBox="0 0 24 24"
          >
            <path d="M22 12h-4l-3 9L9 3l-3 9H2" />
          </svg>
        </div>
        <div class="mt-6 flex-grow text-center sm:mt-0 sm:text-left">
          <h2 class="title-font mb-2 text-lg font-medium text-gray-900 dark:text-white">
            Shooting Stars
          </h2>
          <p class="text-base leading-relaxed">
            Blue bottle crucifix vinyl post-ironic four dollar toast vegan taxidermy. Gastropub indxgo juice poutine.
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
      <div
        class="mx-auto mb-10 flex flex-col items-center border-b border-gray-200 pb-10 lg:w-3/5 sm:flex-row dark:border-gray-800"
      >
        <div class="mt-6 flex-grow text-center sm:mt-0 sm:text-left">
          <h2 class="title-font mb-2 text-lg font-medium text-gray-900 dark:text-white">
            The Catalyzer
          </h2>
          <p class="text-base leading-relaxed">
            Blue bottle crucifix vinyl post-ironic four dollar toast vegan taxidermy. Gastropub indxgo juice poutine.
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
        <div
          :class="`sm:w-32 sm:order-none order-first sm:h-32 h-20 w-20 sm:ml-10 inline-flex items-center justify-center rounded-full bg-${theme}-100 text-${theme}-500 flex-shrink-0 dark:text-${theme}-400 dark:bg-gray-800`"
        >
          <svg
            fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
            class="h-10 w-10 sm:h-16 sm:w-16" viewBox="0 0 24 24"
          >
            <circle cx="6" cy="6" r="3" />
            <circle cx="6" cy="18" r="3" />
            <path d="M20 4L8.12 15.88M14.47 14.48L20 20M8.12 8.12L12 12" />
          </svg>
        </div>
      </div>
      <div class="mx-auto flex flex-col items-center lg:w-3/5 sm:flex-row">
        <div
          :class="`sm:w-32 sm:h-32 h-20 w-20 sm:mr-10 inline-flex items-center justify-center rounded-full bg-${theme}-100 text-${theme}-500 flex-shrink-0 dark:text-${theme}-400 dark:bg-gray-800`"
        >
          <svg
            fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
            class="h-10 w-10 sm:h-16 sm:w-16" viewBox="0 0 24 24"
          >
            <path d="M20 21v-2a4 4 0 00-4-4H8a4 4 0 00-4 4v2" />
            <circle cx="12" cy="7" r="4" />
          </svg>
        </div>
        <div class="mt-6 flex-grow text-center sm:mt-0 sm:text-left">
          <h2 class="title-font mb-2 text-lg font-medium text-gray-900 dark:text-white">
            The 400 Blows
          </h2>
          <p class="text-base leading-relaxed">
            Blue bottle crucifix vinyl post-ironic four dollar toast vegan taxidermy. Gastropub indxgo juice poutine.
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
      <button
        :class="`flex mx-auto mt-20 text-white bg-${theme}-500 border-0 py-2 px-8 focus:outline-none hover:bg-${theme}-600 rounded text-lg`"
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
