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
      <div class="mb-20 w-full flex flex-col text-center">
        <h1 class="title-font mb-2 text-3xl font-medium text-gray-900 sm:text-4xl dark:text-white">
          Pricing
        </h1>
        <p class="mx-auto text-base leading-relaxed text-gray-500 lg:w-2/3">
          Whatever cardigan tote bag tumblr hexagon brooklyn asymmetrical.
        </p>
        <div :class="`flex mx-auto border-2 border-${theme}-500 rounded overflow-hidden mt-6`">
          <button :class="`py-1 px-4 bg-${theme}-500 text-white focus:outline-none`">
            Monthly
          </button>
          <button class="px-4 py-1 dark:text-gray-300 focus:outline-none">
            Annually
          </button>
        </div>
      </div>
      <div class="flex flex-wrap -m-4">
        <div class="w-full p-4 md:w-1/2 xl:w-1/4">
          <div
            class="relative h-full flex flex-col overflow-hidden border-2 border-gray-300 rounded-lg p-6 dark:border-gray-700"
          >
            <h2 class="title-font mb-1 text-sm font-medium tracking-widest dark:text-gray-400">
              START
            </h2>
            <h1
              class="mb-4 border-b border-gray-200 pb-4 text-5xl leading-none text-gray-900 dark:border-gray-800 dark:text-white"
            >
              Free
            </h1>
            <p class="mb-2 flex items-center text-gray-600 dark:text-gray-400">
              <span
                class="mr-2 h-4 w-4 inline-flex flex-shrink-0 items-center justify-center rounded-full bg-gray-400 text-white dark:bg-gray-800 dark:text-gray-500"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Vexillologist pitchfork
            </p>
            <p class="mb-2 flex items-center text-gray-600 dark:text-gray-400">
              <span
                class="mr-2 h-4 w-4 inline-flex flex-shrink-0 items-center justify-center rounded-full bg-gray-400 text-white dark:bg-gray-800 dark:text-gray-500"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Tumeric plaid portland
            </p>
            <p class="mb-6 flex items-center text-gray-600 dark:text-gray-400">
              <span
                class="mr-2 h-4 w-4 inline-flex flex-shrink-0 items-center justify-center rounded-full bg-gray-400 text-white dark:bg-gray-800 dark:text-gray-500"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Mixtape chillwave tumeric
            </p>
            <button
              class="mt-auto w-full flex items-center border-0 rounded bg-gray-400 px-4 py-2 text-white dark:bg-gray-800 hover:bg-gray-500 focus:outline-none dark:hover:bg-gray-700"
            >
              Button
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                class="ml-auto h-4 w-4" viewBox="0 0 24 24"
              >
                <path d="M5 12h14M12 5l7 7-7 7" />
              </svg>
            </button>
            <p class="mt-3 text-xs text-gray-500 dark:text-gray-400">
              Literally you probably haven't heard of them jean shorts.
            </p>
          </div>
        </div>
        <div class="w-full p-4 md:w-1/2 xl:w-1/4">
          <div :class="`h-full p-6 rounded-lg border-2 border-${theme}-500 flex flex-col relative overflow-hidden`">
            <span
              :class="`bg-${theme}-500 text-white px-3 py-1 tracking-widest text-xs absolute right-0 top-0 rounded-bl`"
            >POPULAR</span>
            <h2 class="title-font mb-1 text-sm font-medium tracking-widest dark:text-gray-400">
              PRO
            </h2>
            <h1
              class="mb-4 flex items-center border-b border-gray-200 pb-4 text-5xl leading-none text-gray-900 dark:border-gray-800 dark:text-white"
            >
              <span>$38</span>
              <span class="ml-1 text-lg font-normal text-gray-500 dark:text-gray-400">/mo</span>
            </h1>
            <p class="mb-2 flex items-center text-gray-600 dark:text-gray-400">
              <span
                class="mr-2 h-4 w-4 inline-flex flex-shrink-0 items-center justify-center rounded-full bg-gray-400 text-white dark:bg-gray-800 dark:text-gray-500"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Vexillologist pitchfork
            </p>
            <p class="mb-2 flex items-center text-gray-600 dark:text-gray-400">
              <span
                class="mr-2 h-4 w-4 inline-flex flex-shrink-0 items-center justify-center rounded-full bg-gray-400 text-white dark:bg-gray-800 dark:text-gray-500"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Tumeric plaid portland
            </p>
            <p class="mb-2 flex items-center text-gray-600 dark:text-gray-400">
              <span
                class="mr-2 h-4 w-4 inline-flex flex-shrink-0 items-center justify-center rounded-full bg-gray-400 text-white dark:bg-gray-800 dark:text-gray-500"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Hexagon neutra unicorn
            </p>
            <p class="mb-6 flex items-center text-gray-600 dark:text-gray-400">
              <span
                class="mr-2 h-4 w-4 inline-flex flex-shrink-0 items-center justify-center rounded-full bg-gray-400 text-white dark:bg-gray-800 dark:text-gray-500"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Mixtape chillwave tumeric
            </p>
            <button
              :class="`flex items-center mt-auto text-white bg-${theme}-500 border-0 py-2 px-4 w-full focus:outline-none hover:bg-${theme}-600 rounded`"
            >
              Button
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                class="ml-auto h-4 w-4" viewBox="0 0 24 24"
              >
                <path d="M5 12h14M12 5l7 7-7 7" />
              </svg>
            </button>
            <p class="mt-3 text-xs text-gray-500 dark:text-gray-400">
              Literally you probably haven't heard of them jean shorts.
            </p>
          </div>
        </div>
        <div class="w-full p-4 md:w-1/2 xl:w-1/4">
          <div
            class="relative h-full flex flex-col overflow-hidden border-2 border-gray-300 rounded-lg p-6 dark:border-gray-700"
          >
            <h2 class="title-font mb-1 text-sm font-medium tracking-widest dark:text-gray-400">
              BUSINESS
            </h2>
            <h1
              class="mb-4 flex items-center border-b border-gray-200 pb-4 text-5xl leading-none text-gray-900 dark:border-gray-800 dark:text-white"
            >
              <span>$56</span>
              <span class="ml-1 text-lg font-normal text-gray-500 dark:text-gray-400">/mo</span>
            </h1>
            <p class="mb-2 flex items-center text-gray-600 dark:text-gray-400">
              <span
                class="mr-2 h-4 w-4 inline-flex flex-shrink-0 items-center justify-center rounded-full bg-gray-400 text-white dark:bg-gray-800 dark:text-gray-500"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Vexillologist pitchfork
            </p>
            <p class="mb-2 flex items-center text-gray-600 dark:text-gray-400">
              <span
                class="mr-2 h-4 w-4 inline-flex flex-shrink-0 items-center justify-center rounded-full bg-gray-400 text-white dark:bg-gray-800 dark:text-gray-500"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Tumeric plaid portland
            </p>
            <p class="mb-2 flex items-center text-gray-600 dark:text-gray-400">
              <span
                class="mr-2 h-4 w-4 inline-flex flex-shrink-0 items-center justify-center rounded-full bg-gray-400 text-white dark:bg-gray-800 dark:text-gray-500"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Hexagon neutra unicorn
            </p>
            <p class="mb-2 flex items-center text-gray-600 dark:text-gray-400">
              <span
                class="mr-2 h-4 w-4 inline-flex flex-shrink-0 items-center justify-center rounded-full bg-gray-400 text-white dark:bg-gray-800 dark:text-gray-500"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Vexillologist pitchfork
            </p>
            <p class="mb-6 flex items-center text-gray-600 dark:text-gray-400">
              <span
                class="mr-2 h-4 w-4 inline-flex flex-shrink-0 items-center justify-center rounded-full bg-gray-400 text-white dark:bg-gray-800 dark:text-gray-500"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Mixtape chillwave tumeric
            </p>
            <button
              class="mt-auto w-full flex items-center border-0 rounded bg-gray-400 px-4 py-2 text-white dark:bg-gray-800 hover:bg-gray-500 focus:outline-none dark:hover:bg-gray-700"
            >
              Button
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                class="ml-auto h-4 w-4" viewBox="0 0 24 24"
              >
                <path d="M5 12h14M12 5l7 7-7 7" />
              </svg>
            </button>
            <p class="mt-3 text-xs text-gray-500 dark:text-gray-400">
              Literally you probably haven't heard of them jean shorts.
            </p>
          </div>
        </div>
        <div class="w-full p-4 md:w-1/2 xl:w-1/4">
          <div
            class="relative h-full flex flex-col overflow-hidden border-2 border-gray-300 rounded-lg p-6 dark:border-gray-700"
          >
            <h2 class="title-font mb-1 text-sm font-medium tracking-widest dark:text-gray-400">
              SPECIAL
            </h2>
            <h1
              class="mb-4 flex items-center border-b border-gray-200 pb-4 text-5xl leading-none text-gray-900 dark:border-gray-800 dark:text-white"
            >
              <span>$72</span>
              <span class="ml-1 text-lg font-normal text-gray-500 dark:text-gray-400">/mo</span>
            </h1>
            <p class="mb-2 flex items-center text-gray-600 dark:text-gray-400">
              <span
                class="mr-2 h-4 w-4 inline-flex flex-shrink-0 items-center justify-center rounded-full bg-gray-400 text-white dark:bg-gray-800 dark:text-gray-500"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Vexillologist pitchfork
            </p>
            <p class="mb-2 flex items-center text-gray-600 dark:text-gray-400">
              <span
                class="mr-2 h-4 w-4 inline-flex flex-shrink-0 items-center justify-center rounded-full bg-gray-400 text-white dark:bg-gray-800 dark:text-gray-500"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Tumeric plaid portland
            </p>
            <p class="mb-2 flex items-center text-gray-600 dark:text-gray-400">
              <span
                class="mr-2 h-4 w-4 inline-flex flex-shrink-0 items-center justify-center rounded-full bg-gray-400 text-white dark:bg-gray-800 dark:text-gray-500"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Hexagon neutra unicorn
            </p>
            <p class="mb-2 flex items-center text-gray-600 dark:text-gray-400">
              <span
                class="mr-2 h-4 w-4 inline-flex flex-shrink-0 items-center justify-center rounded-full bg-gray-400 text-white dark:bg-gray-800 dark:text-gray-500"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Vexillologist pitchfork
            </p>
            <p class="mb-6 flex items-center text-gray-600 dark:text-gray-400">
              <span
                class="mr-2 h-4 w-4 inline-flex flex-shrink-0 items-center justify-center rounded-full bg-gray-400 text-white dark:bg-gray-800 dark:text-gray-500"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Mixtape chillwave tumeric
            </p>
            <button
              class="mt-auto w-full flex items-center border-0 rounded bg-gray-400 px-4 py-2 text-white dark:bg-gray-800 hover:bg-gray-500 focus:outline-none dark:hover:bg-gray-700"
            >
              Button
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                class="ml-auto h-4 w-4" viewBox="0 0 24 24"
              >
                <path d="M5 12h14M12 5l7 7-7 7" />
              </svg>
            </button>
            <p class="mt-3 text-xs text-gray-500 dark:text-gray-400">
              Literally you probably haven't heard of them jean shorts.
            </p>
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
