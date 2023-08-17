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
      <div class="mb-10 w-full overflow-hidden rounded-lg lg:mb-0 lg:w-1/2">
        <img alt="feature" class="h-full w-full object-cover object-center" src="https://dummyimage.com/460x500">
      </div>
      <div class="flex flex-col flex-wrap text-center -mb-10 lg:w-1/2 lg:py-6 lg:pl-12 lg:text-left">
        <div class="mb-10 flex flex-col items-center lg:items-start">
          <div
            :class="`w-12 h-12 inline-flex items-center justify-center rounded-full bg-${theme}-100 text-${theme}-500 mb-5 dark:bg-gray-800 dark:text-${theme}-400`"
          >
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              class="h-6 w-6" viewBox="0 0 24 24"
            >
              <path d="M22 12h-4l-3 9L9 3l-3 9H2" />
            </svg>
          </div>
          <div class="flex-grow">
            <h2 class="title-font mb-3 text-lg font-medium text-gray-900 dark:text-white">
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
        <div class="mb-10 flex flex-col items-center lg:items-start">
          <div
            :class="`w-12 h-12 inline-flex items-center justify-center rounded-full bg-${theme}-100 text-${theme}-500 mb-5 dark:bg-gray-800 dark:text-${theme}-400`"
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
          <div class="flex-grow">
            <h2 class="title-font mb-3 text-lg font-medium text-gray-900 dark:text-white">
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
        </div>
        <div class="mb-10 flex flex-col items-center lg:items-start">
          <div
            :class="`w-12 h-12 inline-flex items-center justify-center rounded-full bg-${theme}-100 text-${theme}-500 mb-5 dark:bg-gray-800 dark:text-${theme}-400`"
          >
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              class="h-6 w-6" viewBox="0 0 24 24"
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
      </div>
    </div>
  </section>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>

<style></style>
