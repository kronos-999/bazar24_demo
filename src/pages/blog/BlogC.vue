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
      <div class="flex flex-wrap -m-12">
        <div class="flex flex-col items-start p-12 md:w-1/2">
          <span
            :class="`inline-block py-1 px-2 rounded bg-${theme}-50 text-${theme}-500 text-xs font-medium tracking-widest dark:bg-gray-800 dark:text-gray-400 dark:text-opacity-75`"
          >CATEGORY</span>
          <h2 class="title-font mb-4 mt-4 text-2xl font-medium text-gray-900 sm:text-3xl dark:text-white">
            Roof party normcore before they sold out, cornhole vape
          </h2>
          <p class="mb-8 leading-relaxed">
            Live-edge letterpress cliche, salvia fanny pack humblebrag narwhal portland. VHS man braid palo santo hoodie
            brunch trust fund. Bitters hashtag waistcoat fashion axe chia unicorn. Plaid fixie chambray 90's, slow-carb
            etsy tumeric. Cray pug you probably haven't heard of them hexagon kickstarter craft beer pork chic.
          </p>
          <div
            class="mb-4 mt-auto w-full flex flex-wrap items-center border-b-2 border-gray-100 pb-4 dark:border-gray-800 dark:border-opacity-75"
          >
            <a :class="`text-${theme}-500 inline-flex items-center dark:text-${theme}-400`">Learn More
              <svg
                class="ml-2 h-4 w-4" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2" fill="none"
                stroke-linecap="round" stroke-linejoin="round"
              >
                <path d="M5 12h14" />
                <path d="M12 5l7 7-7 7" />
              </svg>
            </a>
            <span
              class="ml-auto mr-3 inline-flex items-center border-r-2 border-gray-200 py-1 pr-3 text-sm leading-none text-gray-400 dark:border-gray-800 dark:text-gray-500"
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
          <a class="inline-flex items-center">
            <img
              alt="blog" src="https://dummyimage.com/104x104"
              class="h-12 w-12 flex-shrink-0 rounded-full object-cover object-center"
            >
            <span class="flex flex-grow flex-col pl-4">
              <span class="title-font font-medium text-gray-900 dark:text-white">Holden Caulfield</span>
              <span class="mt-0.5 text-xs tracking-widest text-gray-400 dark:text-gray-500">UI DEVELOPER</span>
            </span>
          </a>
        </div>
        <div class="flex flex-col items-start p-12 md:w-1/2">
          <span
            :class="`inline-block py-1 px-2 rounded bg-${theme}-50 text-${theme}-500 text-xs font-medium tracking-widest dark:bg-gray-800 dark:text-gray-400 dark:text-opacity-75`"
          >CATEGORY</span>
          <h2 class="title-font mb-4 mt-4 text-2xl font-medium text-gray-900 sm:text-3xl dark:text-white">
            Pinterest DIY dreamcatcher gentrify single-origin coffee
          </h2>
          <p class="mb-8 leading-relaxed">
            Live-edge letterpress cliche, salvia fanny pack humblebrag narwhal portland. VHS man braid palo santo hoodie
            brunch trust fund. Bitters hashtag waistcoat fashion axe chia unicorn. Plaid fixie chambray 90's, slow-carb
            etsy tumeric.
          </p>
          <div
            class="mb-4 mt-auto w-full flex flex-wrap items-center border-b-2 border-gray-100 pb-4 dark:border-gray-800 dark:border-opacity-75"
          >
            <a :class="`text-${theme}-500 inline-flex items-center dark:text-${theme}-400`">Learn More
              <svg
                class="ml-2 h-4 w-4" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2" fill="none"
                stroke-linecap="round" stroke-linejoin="round"
              >
                <path d="M5 12h14" />
                <path d="M12 5l7 7-7 7" />
              </svg>
            </a>
            <span
              class="ml-auto mr-3 inline-flex items-center border-r-2 border-gray-200 py-1 pr-3 text-sm leading-none text-gray-400 dark:border-gray-800 dark:text-gray-500"
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
          <a class="inline-flex items-center">
            <img
              alt="blog" src="https://dummyimage.com/103x103"
              class="h-12 w-12 flex-shrink-0 rounded-full object-cover object-center"
            >
            <span class="flex flex-grow flex-col pl-4">
              <span class="title-font font-medium text-gray-900 dark:text-white">Alper Kamu</span>
              <span class="mt-0.5 text-xs tracking-widest text-gray-400 dark:text-gray-500">DESIGNER</span>
            </span>
          </a>
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
