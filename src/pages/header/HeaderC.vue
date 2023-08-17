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
  <header class="body-font text-gray-600 dark:bg-gray-900 dark:text-gray-400">
    <div class="mx-auto flex flex-col flex-wrap items-center p-5 container md:flex-row">
      <nav class="flex flex-wrap items-center text-base md:ml-auto lg:w-2/5">
        <a class="mr-5 hover:text-gray-900 dark:hover:text-white">First Link</a>
        <a class="mr-5 hover:text-gray-900 dark:hover:text-white">Second Link</a>
        <a class="mr-5 hover:text-gray-900 dark:hover:text-white">Third Link</a>
        <a class="hover:text-gray-900 dark:hover:text-white">Fourth Link</a>
      </nav>
      <a
        class="title-font order-first mb-4 flex items-center font-medium text-gray-900 lg:order-none md:mb-0 lg:w-1/5 lg:items-center lg:justify-center dark:text-white"
      >
        <svg
          xmlns="http://www.w3.org/2000/svg" fill="none" stroke="currentColor" stroke-linecap="round"
          stroke-linejoin="round" stroke-width="2" :class="`w-10 h-10 text-white p-2 bg-${theme}-500 rounded-full`"
          viewBox="0 0 24 24"
        >
          <path d="M12 2L2 7l10 5 10-5-10-5zM2 17l10 5 10-5M2 12l10 5 10-5" />
        </svg>
        <span class="ml-3 text-xl dark:xl:block dark:lg:hidden">Tailblocks</span>
      </a>
      <div class="ml-5 inline-flex lg:ml-0 lg:w-2/5 lg:justify-end">
        <button
          class="mt-4 inline-flex items-center border-0 rounded bg-gray-100 px-3 py-1 text-base md:mt-0 dark:bg-gray-800 hover:bg-gray-200 focus:outline-none dark:hover:bg-gray-700"
        >
          Button
          <svg
            fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
            class="ml-1 h-4 w-4" viewBox="0 0 24 24"
          >
            <path d="M5 12h14M12 5l7 7-7 7" />
          </svg>
        </button>
      </div>
    </div>
  </header>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>

<style></style>
