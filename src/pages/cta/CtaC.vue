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
      <div class="mb-12 w-full flex flex-col text-center">
        <h1 class="title-font mb-4 text-2xl font-medium text-gray-900 sm:text-3xl dark:text-white">
          Master Cleanse Reliac Heirloom
        </h1>
        <p class="mx-auto text-base leading-relaxed lg:w-2/3">
          Whatever cardigan tote bag tumblr hexagon brooklyn asymmetrical gentrify, subway tile poke farm-to-table.
          Franzen you probably haven't heard of them man bun deep.
        </p>
      </div>
      <div
        class="mx-auto w-full flex flex-col items-end px-8 lg:w-2/3 sm:flex-row space-y-4 sm:px-0 sm:space-x-4 sm:space-y-0"
      >
        <div class="relative w-full flex-grow dark:sm:mb-0">
          <label for="full-name" class="text-sm leading-7 text-gray-600 dark:text-gray-400">Full Name</label>
          <input
            id="full-name" type="text" name="full-name"
            :class="`w-full bg-gray-100 bg-opacity-50 rounded border border-gray-300 focus:border-${theme}-500 focus:bg-transparent focus:ring-2 focus:ring-${theme}-200 text-base outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out dark:bg-gray-800 dark:bg-opacity-40 dark:border-gray-700 dark:focus:ring-${theme}-900 dark:text-gray-100`"
          >
        </div>
        <div class="relative w-full flex-grow dark:sm:mb-0">
          <label for="email" class="text-sm leading-7 text-gray-600 dark:text-gray-400">Email</label>
          <input
            id="email" type="email" name="email"
            :class="`w-full bg-gray-100 bg-opacity-50 rounded border border-gray-300 focus:border-${theme}-500 focus:bg-transparent focus:ring-2 focus:ring-${theme}-200 text-base outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out dark:bg-gray-800 dark:bg-opacity-40 dark:border-gray-700 dark:focus:ring-${theme}-900 dark:text-gray-100`"
          >
        </div>
        <button
          :class="`text-white bg-${theme}-500 border-0 py-2 px-8 focus:outline-none hover:bg-${theme}-600 rounded text-lg`"
        >
          Button
        </button>
      </div>
    </div>
  </section>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>

<style></style>
