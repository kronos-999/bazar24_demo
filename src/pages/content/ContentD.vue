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
    <div class="mx-auto flex flex-wrap items-center px-5 py-24 container">
      <div
        class="mb-10 border-b border-gray-200 pb-10 md:mb-0 md:w-1/2 md:border-b-0 md:border-r dark:border-gray-800 md:py-8 md:pr-12"
      >
        <h1 class="title-font mb-2 text-2xl font-medium text-gray-900 sm:text-3xl dark:text-white">
          Pitchfork Kickstarter Taxidermy
        </h1>
        <p class="text-base leading-relaxed">
          Locavore cardigan small batch roof party blue bottle blog meggings sartorial jean shorts kickstarter migas
          sriracha church-key synth succulents. Actually taiyaki neutra, distillery gastropub pok pok ugh.
        </p>
        <a :class="`text-${theme}-500 inline-flex items-center mt-4 dark:text-${theme}-400`">Learn More
          <svg
            fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
            class="ml-2 h-4 w-4" viewBox="0 0 24 24"
          >
            <path d="M5 12h14M12 5l7 7-7 7" />
          </svg>
        </a>
      </div>
      <div class="flex flex-col md:w-1/2 md:pl-12">
        <h2 class="title-font mb-3 text-sm font-semibold tracking-wider text-gray-800 dark:text-white">
          CATEGORIES
        </h2>
        <nav class="flex flex-wrap list-none -mb-1">
          <li class="mb-1 w-1/2 lg:w-1/3">
            <a class="text-gray-600 hover:text-gray-800 dark:hover:text-white">First Link</a>
          </li>
          <li class="mb-1 w-1/2 lg:w-1/3">
            <a class="text-gray-600 hover:text-gray-800 dark:hover:text-white">Second Link</a>
          </li>
          <li class="mb-1 w-1/2 lg:w-1/3">
            <a class="text-gray-600 hover:text-gray-800 dark:hover:text-white">Third Link</a>
          </li>
          <li class="mb-1 w-1/2 lg:w-1/3">
            <a class="text-gray-600 hover:text-gray-800 dark:hover:text-white">Fourth Link</a>
          </li>
          <li class="mb-1 w-1/2 lg:w-1/3">
            <a class="text-gray-600 hover:text-gray-800 dark:hover:text-white">Fifth Link</a>
          </li>
          <li class="mb-1 w-1/2 lg:w-1/3">
            <a class="text-gray-600 hover:text-gray-800 dark:hover:text-white">Sixth Link</a>
          </li>
          <li class="mb-1 w-1/2 lg:w-1/3">
            <a class="text-gray-600 hover:text-gray-800 dark:hover:text-white">Seventh Link</a>
          </li>
          <li class="mb-1 w-1/2 lg:w-1/3">
            <a class="text-gray-600 hover:text-gray-800 dark:hover:text-white">Eighth Link</a>
          </li>
        </nav>
      </div>
    </div>
  </section>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>

<style></style>
