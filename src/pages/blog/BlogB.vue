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
      <div class="flex flex-wrap -m-4">
        <div class="p-4 lg:w-1/3">
          <div
            class="relative h-full overflow-hidden rounded-lg bg-gray-100 bg-opacity-75 px-8 pb-24 pt-16 text-center dark:bg-gray-800 dark:bg-opacity-40"
          >
            <h2 class="title-font mb-1 text-xs font-medium tracking-widest text-gray-400 dark:text-gray-500">
              CATEGORY
            </h2>
            <h1 class="title-font mb-3 text-xl font-medium text-gray-900 sm:text-2xl dark:text-white">
              Raclette Blueberry Nextious Level
            </h1>
            <p class="mb-3 leading-relaxed">
              Photo booth fam kinfolk cold-pressed sriracha leggings jianbing microdosing tousled waistcoat.
            </p>
            <a :class="`text-${theme}-500 inline-flex items-center dark:text-${theme}-400`">Learn More
              <svg
                class="ml-2 h-4 w-4" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2" fill="none"
                stroke-linecap="round" stroke-linejoin="round"
              >
                <path d="M5 12h14" />
                <path d="M12 5l7 7-7 7" />
              </svg>
            </a>
            <div class="absolute bottom-0 left-0 mt-2 w-full flex justify-center py-4 text-center leading-none">
              <span
                class="mr-3 inline-flex items-center border-r-2 border-gray-200 py-1 pr-3 text-sm leading-none text-gray-400 dark:border-gray-700 dark:border-opacity-50 dark:text-gray-500"
              >
                <svg
                  class="mr-1 h-4 w-4" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round"
                  stroke-linejoin="round" viewBox="0 0 24 24"
                >
                  <path d="M1 12s4-8 11-8 11 8 11 8-4 8-11 8-11-8-11-8z" />
                  <circle cx="12" cy="12" r="3" />
                </svg>1.2K
              </span>
              <span class="inline-flex items-center text-sm leading-none text-gray-400 dark:text-gray-500">
                <svg
                  class="mr-1 h-4 w-4" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round"
                  stroke-linejoin="round" viewBox="0 0 24 24"
                >
                  <path
                    d="M21 11.5a8.38 8.38 0 01-.9 3.8 8.5 8.5 0 01-7.6 4.7 8.38 8.38 0 01-3.8-.9L3 21l1.9-5.7a8.38 8.38 0 01-.9-3.8 8.5 8.5 0 014.7-7.6 8.38 8.38 0 013.8-.9h.5a8.48 8.48 0 018 8v.5z"
                  />
                </svg>6
              </span>
            </div>
          </div>
        </div>
        <div class="p-4 lg:w-1/3">
          <div
            class="relative h-full overflow-hidden rounded-lg bg-gray-100 bg-opacity-75 px-8 pb-24 pt-16 text-center dark:bg-gray-800 dark:bg-opacity-40"
          >
            <h2 class="title-font mb-1 text-xs font-medium tracking-widest text-gray-400 dark:text-gray-500">
              CATEGORY
            </h2>
            <h1 class="title-font mb-3 text-xl font-medium text-gray-900 sm:text-2xl dark:text-white">
              Ennui Snackwave Thundercats
            </h1>
            <p class="mb-3 leading-relaxed">
              Photo booth fam kinfolk cold-pressed sriracha leggings jianbing microdosing tousled waistcoat.
            </p>
            <a :class="`text-${theme}-500 inline-flex items-center dark:text-${theme}-400`">Learn More
              <svg
                class="ml-2 h-4 w-4" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2" fill="none"
                stroke-linecap="round" stroke-linejoin="round"
              >
                <path d="M5 12h14" />
                <path d="M12 5l7 7-7 7" />
              </svg>
            </a>
            <div class="absolute bottom-0 left-0 mt-2 w-full flex justify-center py-4 text-center leading-none">
              <span
                class="mr-3 inline-flex items-center border-r-2 border-gray-200 py-1 pr-3 text-sm leading-none text-gray-400 dark:border-gray-700 dark:border-opacity-50 dark:text-gray-500"
              >
                <svg
                  class="mr-1 h-4 w-4" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round"
                  stroke-linejoin="round" viewBox="0 0 24 24"
                >
                  <path d="M1 12s4-8 11-8 11 8 11 8-4 8-11 8-11-8-11-8z" />
                  <circle cx="12" cy="12" r="3" />
                </svg>1.2K
              </span>
              <span class="inline-flex items-center text-sm leading-none text-gray-400 dark:text-gray-500">
                <svg
                  class="mr-1 h-4 w-4" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round"
                  stroke-linejoin="round" viewBox="0 0 24 24"
                >
                  <path
                    d="M21 11.5a8.38 8.38 0 01-.9 3.8 8.5 8.5 0 01-7.6 4.7 8.38 8.38 0 01-3.8-.9L3 21l1.9-5.7a8.38 8.38 0 01-.9-3.8 8.5 8.5 0 014.7-7.6 8.38 8.38 0 013.8-.9h.5a8.48 8.48 0 018 8v.5z"
                  />
                </svg>6
              </span>
            </div>
          </div>
        </div>
        <div class="p-4 lg:w-1/3">
          <div
            class="relative h-full overflow-hidden rounded-lg bg-gray-100 bg-opacity-75 px-8 pb-24 pt-16 text-center dark:bg-gray-800 dark:bg-opacity-40"
          >
            <h2 class="title-font mb-1 text-xs font-medium tracking-widest text-gray-400 dark:text-gray-500">
              CATEGORY
            </h2>
            <h1 class="title-font mb-3 text-xl font-medium text-gray-900 sm:text-2xl dark:text-white">
              Selvage Poke Waistcoat Godard
            </h1>
            <p class="mb-3 leading-relaxed">
              Photo booth fam kinfolk cold-pressed sriracha leggings jianbing microdosing tousled waistcoat.
            </p>
            <a :class="`text-${theme}-500 inline-flex items-center dark:text-${theme}-400`">Learn More
              <svg
                class="ml-2 h-4 w-4" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2" fill="none"
                stroke-linecap="round" stroke-linejoin="round"
              >
                <path d="M5 12h14" />
                <path d="M12 5l7 7-7 7" />
              </svg>
            </a>
            <div class="absolute bottom-0 left-0 mt-2 w-full flex justify-center py-4 text-center leading-none">
              <span
                class="mr-3 inline-flex items-center border-r-2 border-gray-200 py-1 pr-3 text-sm leading-none text-gray-400 dark:border-gray-700 dark:border-opacity-50 dark:text-gray-500"
              >
                <svg
                  class="mr-1 h-4 w-4" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round"
                  stroke-linejoin="round" viewBox="0 0 24 24"
                >
                  <path d="M1 12s4-8 11-8 11 8 11 8-4 8-11 8-11-8-11-8z" />
                  <circle cx="12" cy="12" r="3" />
                </svg>1.2K
              </span>
              <span class="inline-flex items-center text-sm leading-none text-gray-400 dark:text-gray-500">
                <svg
                  class="mr-1 h-4 w-4" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round"
                  stroke-linejoin="round" viewBox="0 0 24 24"
                >
                  <path
                    d="M21 11.5a8.38 8.38 0 01-.9 3.8 8.5 8.5 0 01-7.6 4.7 8.38 8.38 0 01-3.8-.9L3 21l1.9-5.7a8.38 8.38 0 01-.9-3.8 8.5 8.5 0 014.7-7.6 8.38 8.38 0 013.8-.9h.5a8.48 8.48 0 018 8v.5z"
                  />
                </svg>6
              </span>
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
