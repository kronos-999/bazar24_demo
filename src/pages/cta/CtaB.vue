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
      <div class="pr-0 lg:w-3/5 md:w-1/2 lg:pr-0 md:pr-16">
        <h1 class="title-font text-3xl font-medium text-gray-900 dark:text-white">
          Slow-carb next level shoindcgoitch ethical authentic, poko scenester
        </h1>
        <p class="mt-4 leading-relaxed">
          Poke slow-carb mixtape knausgaard, typewriter street art gentrify hammock starladder roathse. Craies vegan
          tousled etsy austin.
        </p>
      </div>
      <div
        class="mt-10 w-full flex flex-col rounded-lg bg-gray-100 p-8 md:ml-auto md:mt-0 lg:w-2/6 md:w-1/2 dark:bg-gray-800 dark:bg-opacity-50"
      >
        <h2 class="title-font mb-5 text-lg font-medium text-gray-900 dark:text-white">
          Sign Up
        </h2>
        <div class="relative mb-4">
          <label for="full-name" class="text-sm leading-7 text-gray-600 dark:text-gray-400">Full Name</label>
          <input
            id="full-name" type="text" name="full-name"
            :class="`w-full bg-white rounded border border-gray-300 focus:border-${theme}-500 focus:ring-2 focus:ring-${theme}-200 text-base outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out dark:bg-gray-600 dark:bg-opacity-20 dark:focus:bg-transparent dark:focus:ring-${theme}-900 dark:border-gray-600 dark:text-gray-100`"
          >
        </div>
        <div class="relative mb-4">
          <label for="email" class="text-sm leading-7 text-gray-600 dark:text-gray-400">Email</label>
          <input
            id="email" type="email" name="email"
            :class="`w-full bg-white rounded border border-gray-300 focus:border-${theme}-500 focus:ring-2 focus:ring-${theme}-200 text-base outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out dark:bg-gray-600 dark:bg-opacity-20 dark:focus:bg-transparent dark:focus:ring-${theme}-900 dark:border-gray-600 dark:text-gray-100`"
          >
        </div>
        <button
          :class="`text-white bg-${theme}-500 border-0 py-2 px-8 focus:outline-none hover:bg-${theme}-600 rounded text-lg`"
        >
          Button
        </button>
        <p class="mt-3 text-xs text-gray-500">
          Literally you probably haven't heard of them jean shorts.
        </p>
      </div>
    </div>
  </section>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>

<style></style>
