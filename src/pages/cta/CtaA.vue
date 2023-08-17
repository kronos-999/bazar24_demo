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
      <div class="mx-auto flex flex-col items-start lg:w-2/3 sm:flex-row sm:items-center">
        <h1 class="title-font flex-grow text-2xl font-medium text-gray-900 sm:pr-16 dark:text-white">
          Slow-carb next level shoindxgoitch ethical authentic, scenester sriracha forage.
        </h1>
        <button
          :class="`flex-shrink-0 text-white bg-${theme}-500 border-0 py-2 px-8 focus:outline-none hover:bg-${theme}-600 rounded text-lg mt-10 sm:mt-0`"
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
