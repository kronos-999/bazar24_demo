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
        <h1 class="title-font mb-4 text-center text-2xl font-medium text-gray-900 sm:text-3xl dark:text-white">
          Raw Denim Heirloom Man Braid
        </h1>
        <p class="mx-auto text-base leading-relaxed lg:w-3/4 xl:w-2/4">
          Blue bottle crucifix vinyl post-ironic four dollar toast vegan taxidermy. Gastropub indxgo juice poutine,
          ramps microdosing banh mi pug.
        </p>
      </div>
      <div class="flex flex-wrap -m-4">
        <div class="w-full p-4 lg:w-1/4 sm:w-1/2">
          <h2
            class="title-font mb-4 text-center text-sm font-medium tracking-widest text-gray-900 sm:text-left dark:text-white"
          >
            SHOOTING STARS
          </h2>
          <nav
            class="flex flex-col items-center text-center -mb-1 sm:items-start space-y-2.5 sm:text-left dark:space-y-2"
          >
            <a>
              <span
                :class="`bg-${theme}-100 text-${theme}-500 w-4 h-4 mr-2 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>First Link
            </a>
            <a>
              <span
                :class="`bg-${theme}-100 text-${theme}-500 w-4 h-4 mr-2 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Second Link
            </a>
            <a>
              <span
                :class="`bg-${theme}-100 text-${theme}-500 w-4 h-4 mr-2 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Third Link
            </a>
            <a>
              <span
                :class="`bg-${theme}-100 text-${theme}-500 w-4 h-4 mr-2 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Fourth Link
            </a>
            <a>
              <span
                :class="`bg-${theme}-100 text-${theme}-500 w-4 h-4 mr-2 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Fifth Link
            </a>
          </nav>
        </div>
        <div class="w-full p-4 lg:w-1/4 sm:w-1/2">
          <h2
            class="title-font mb-4 text-center text-sm font-medium tracking-widest text-gray-900 sm:text-left dark:text-white"
          >
            THE 400 BLOWS
          </h2>
          <nav
            class="flex flex-col items-center text-center -mb-1 sm:items-start space-y-2.5 sm:text-left dark:space-y-2"
          >
            <a>
              <span
                :class="`bg-${theme}-100 text-${theme}-500 w-4 h-4 mr-2 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>First Link
            </a>
            <a>
              <span
                :class="`bg-${theme}-100 text-${theme}-500 w-4 h-4 mr-2 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Second Link
            </a>
            <a>
              <span
                :class="`bg-${theme}-100 text-${theme}-500 w-4 h-4 mr-2 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Third Link
            </a>
            <a>
              <span
                :class="`bg-${theme}-100 text-${theme}-500 w-4 h-4 mr-2 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Fourth Link
            </a>
            <a>
              <span
                :class="`bg-${theme}-100 text-${theme}-500 w-4 h-4 mr-2 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Fifth Link
            </a>
          </nav>
        </div>
        <div class="w-full p-4 lg:w-1/4 sm:w-1/2">
          <h2
            class="title-font mb-4 text-center text-sm font-medium tracking-widest text-gray-900 sm:text-left dark:text-white"
          >
            THE CATALYZER
          </h2>
          <nav
            class="flex flex-col items-center text-center -mb-1 sm:items-start space-y-2.5 sm:text-left dark:space-y-2"
          >
            <a>
              <span
                :class="`bg-${theme}-100 text-${theme}-500 w-4 h-4 mr-2 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>First Link
            </a>
            <a>
              <span
                :class="`bg-${theme}-100 text-${theme}-500 w-4 h-4 mr-2 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Second Link
            </a>
            <a>
              <span
                :class="`bg-${theme}-100 text-${theme}-500 w-4 h-4 mr-2 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Third Link
            </a>
            <a>
              <span
                :class="`bg-${theme}-100 text-${theme}-500 w-4 h-4 mr-2 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Fourth Link
            </a>
            <a>
              <span
                :class="`bg-${theme}-100 text-${theme}-500 w-4 h-4 mr-2 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Fifth Link
            </a>
          </nav>
        </div>
        <div class="w-full p-4 lg:w-1/4 sm:w-1/2">
          <h2
            class="title-font mb-4 text-center text-sm font-medium tracking-widest text-gray-900 sm:text-left dark:text-white"
          >
            NEPTUNE
          </h2>
          <nav
            class="flex flex-col items-center text-center -mb-1 sm:items-start space-y-2.5 sm:text-left dark:space-y-2"
          >
            <a>
              <span
                :class="`bg-${theme}-100 text-${theme}-500 w-4 h-4 mr-2 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>First Link
            </a>
            <a>
              <span
                :class="`bg-${theme}-100 text-${theme}-500 w-4 h-4 mr-2 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Second Link
            </a>
            <a>
              <span
                :class="`bg-${theme}-100 text-${theme}-500 w-4 h-4 mr-2 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Third Link
            </a>
            <a>
              <span
                :class="`bg-${theme}-100 text-${theme}-500 w-4 h-4 mr-2 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Fourth Link
            </a>
            <a>
              <span
                :class="`bg-${theme}-100 text-${theme}-500 w-4 h-4 mr-2 rounded-full inline-flex items-center justify-center dark:bg-gray-800 dark:text-${theme}-400`"
              >
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3"
                  class="h-3 w-3" viewBox="0 0 24 24"
                >
                  <path d="M20 6L9 17l-5-5" />
                </svg> </span>Fifth Link
            </a>
          </nav>
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
