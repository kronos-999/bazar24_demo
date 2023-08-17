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
        <div class="p-4 md:w-1/3">
          <div class="h-full overflow-hidden border-2 border-gray-200 border-opacity-60 rounded-lg dark:border-gray-800">
            <img
              class="w-full object-cover object-center lg:h-48 md:h-36" src="https://dummyimage.com/720x400"
              alt="blog"
            >
            <div class="p-6">
              <h2 class="title-font mb-1 text-xs font-medium tracking-widest text-gray-400 dark:text-gray-500">
                CATEGORY
              </h2>
              <h1 class="title-font mb-3 text-lg font-medium text-gray-900 dark:text-white">
                The Catalyzer
              </h1>
              <p class="mb-3 leading-relaxed">
                Photo booth fam kinfolk cold-pressed sriracha leggings jianbing microdosing tousled waistcoat.
              </p>
              <div class="flex flex-wrap items-center">
                <a :class="`text-${theme}-500 inline-flex items-center md:mb-2 lg:mb-0 dark:text-${theme}-400`">Learn More
                  <svg
                    class="ml-2 h-4 w-4" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2" fill="none"
                    stroke-linecap="round" stroke-linejoin="round"
                  >
                    <path d="M5 12h14" />
                    <path d="M12 5l7 7-7 7" />
                  </svg>
                </a>
                <span
                  class="ml-auto mr-3 inline-flex items-center border-r-2 border-gray-200 py-1 pr-3 text-sm leading-none text-gray-400 lg:ml-auto md:ml-0 dark:border-gray-800 dark:text-gray-500"
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
        <div class="p-4 md:w-1/3">
          <div class="h-full overflow-hidden border-2 border-gray-200 border-opacity-60 rounded-lg dark:border-gray-800">
            <img
              class="w-full object-cover object-center lg:h-48 md:h-36" src="https://dummyimage.com/721x401"
              alt="blog"
            >
            <div class="p-6">
              <h2 class="title-font mb-1 text-xs font-medium tracking-widest text-gray-400 dark:text-gray-500">
                CATEGORY
              </h2>
              <h1 class="title-font mb-3 text-lg font-medium text-gray-900 dark:text-white">
                The 400 Blows
              </h1>
              <p class="mb-3 leading-relaxed">
                Photo booth fam kinfolk cold-pressed sriracha leggings jianbing microdosing tousled waistcoat.
              </p>
              <div class="flex flex-wrap items-center">
                <a :class="`text-${theme}-500 inline-flex items-center md:mb-2 lg:mb-0 dark:text-${theme}-400`">Learn More
                  <svg
                    class="ml-2 h-4 w-4" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2" fill="none"
                    stroke-linecap="round" stroke-linejoin="round"
                  >
                    <path d="M5 12h14" />
                    <path d="M12 5l7 7-7 7" />
                  </svg>
                </a>
                <span
                  class="ml-auto mr-3 inline-flex items-center border-r-2 border-gray-200 py-1 pr-3 text-sm leading-none text-gray-400 lg:ml-auto md:ml-0 dark:border-gray-800 dark:text-gray-500"
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
        <div class="p-4 md:w-1/3">
          <div class="h-full overflow-hidden border-2 border-gray-200 border-opacity-60 rounded-lg dark:border-gray-800">
            <img
              class="w-full object-cover object-center lg:h-48 md:h-36" src="https://dummyimage.com/722x402"
              alt="blog"
            >
            <div class="p-6">
              <h2 class="title-font mb-1 text-xs font-medium tracking-widest text-gray-400 dark:text-gray-500">
                CATEGORY
              </h2>
              <h1 class="title-font mb-3 text-lg font-medium text-gray-900 dark:text-white">
                Shooting Stars
              </h1>
              <p class="mb-3 leading-relaxed">
                Photo booth fam kinfolk cold-pressed sriracha leggings jianbing microdosing tousled waistcoat.
              </p>
              <div class="flex flex-wrap items-center">
                <a :class="`text-${theme}-500 inline-flex items-center md:mb-2 lg:mb-0 dark:text-${theme}-400`">Learn More
                  <svg
                    class="ml-2 h-4 w-4" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2" fill="none"
                    stroke-linecap="round" stroke-linejoin="round"
                  >
                    <path d="M5 12h14" />
                    <path d="M12 5l7 7-7 7" />
                  </svg>
                </a>
                <span
                  class="ml-auto mr-3 inline-flex items-center border-r-2 border-gray-200 py-1 pr-3 text-sm leading-none text-gray-400 lg:ml-auto md:ml-0 dark:border-gray-800 dark:text-gray-500"
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
    </div>
  </section>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>

<style></style>
