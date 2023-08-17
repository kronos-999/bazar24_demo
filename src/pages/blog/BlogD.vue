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
  <section class="body-font overflow-hidden text-gray-600 dark:bg-gray-900 dark:text-gray-400">
    <div class="mx-auto px-5 py-24 container">
      <div class="-my-8 divide-y-2 divide-gray-100 dark:divide-gray-800">
        <div class="flex flex-wrap py-8 md:flex-nowrap">
          <div class="mb-6 flex flex-shrink-0 flex-col md:mb-0 md:w-64">
            <span class="title-font font-semibold text-gray-700 dark:text-white">CATEGORY</span>
            <span class="mt-1 text-sm text-gray-500">12 Jun 2019</span>
          </div>
          <div class="md:flex-grow">
            <h2 class="title-font mb-2 text-2xl font-medium text-gray-900 dark:text-white">
              Bitters hashtag waistcoat fashion axe chia unicorn
            </h2>
            <p class="leading-relaxed">
              Glossier echo park pug, church-key sartorial biodiesel vexillologist pop-up snackwave ramps cornhole.
              Marfa 3 wolf moon party messenger bag selfies, poke vaporware kombucha lumbersexual pork belly polaroid
              hoodie portland craft beer.
            </p>
            <a :class="`text-${theme}-500 inline-flex items-center mt-4 dark:text-${theme}-400`">Learn More
              <svg
                class="ml-2 h-4 w-4" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2" fill="none"
                stroke-linecap="round" stroke-linejoin="round"
              >
                <path d="M5 12h14" />
                <path d="M12 5l7 7-7 7" />
              </svg>
            </a>
          </div>
        </div>
        <div class="flex flex-wrap py-8 md:flex-nowrap dark:border-t-2 dark:border-gray-800">
          <div class="mb-6 flex flex-shrink-0 flex-col md:mb-0 md:w-64">
            <span class="title-font font-semibold text-gray-700 dark:text-white">CATEGORY</span>
            <span class="mt-1 text-sm text-gray-500">12 Jun 2019</span>
          </div>
          <div class="md:flex-grow">
            <h2 class="title-font mb-2 text-2xl font-medium text-gray-900 dark:text-white">
              Meditation bushwick direct trade taxidermy shaman
            </h2>
            <p class="leading-relaxed">
              Glossier echo park pug, church-key sartorial biodiesel vexillologist pop-up snackwave ramps cornhole.
              Marfa 3 wolf moon party messenger bag selfies, poke vaporware kombucha lumbersexual pork belly polaroid
              hoodie portland craft beer.
            </p>
            <a :class="`text-${theme}-500 inline-flex items-center mt-4 dark:text-${theme}-400`">Learn More
              <svg
                class="ml-2 h-4 w-4" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2" fill="none"
                stroke-linecap="round" stroke-linejoin="round"
              >
                <path d="M5 12h14" />
                <path d="M12 5l7 7-7 7" />
              </svg>
            </a>
          </div>
        </div>
        <div class="flex flex-wrap py-8 md:flex-nowrap dark:border-t-2 dark:border-gray-800">
          <div class="mb-6 flex flex-shrink-0 flex-col md:mb-0 md:w-64">
            <span class="title-font font-semibold text-gray-700 dark:text-white">CATEGORY</span>
            <span class="text-sm text-gray-500 dark:mt-1">12 Jun 2019</span>
          </div>
          <div class="md:flex-grow">
            <h2 class="title-font mb-2 text-2xl font-medium text-gray-900 dark:text-white">
              Woke master cleanse drinking vinegar salvia
            </h2>
            <p class="leading-relaxed">
              Glossier echo park pug, church-key sartorial biodiesel vexillologist pop-up snackwave ramps cornhole.
              Marfa 3 wolf moon party messenger bag selfies, poke vaporware kombucha lumbersexual pork belly polaroid
              hoodie portland craft beer.
            </p>
            <a :class="`text-${theme}-500 inline-flex items-center mt-4 dark:text-${theme}-400`">Learn More
              <svg
                class="ml-2 h-4 w-4" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2" fill="none"
                stroke-linecap="round" stroke-linejoin="round"
              >
                <path d="M5 12h14" />
                <path d="M12 5l7 7-7 7" />
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
