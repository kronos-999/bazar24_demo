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
      <div class="flex flex-wrap text-center -mx-4 -mb-10">
        <div class="mb-10 px-4 sm:w-1/2">
          <div class="h-64 overflow-hidden rounded-lg">
            <img alt="content" class="h-full w-full object-cover object-center" src="https://dummyimage.com/1201x501">
          </div>
          <h2 class="title-font mb-3 mt-6 text-2xl font-medium text-gray-900 dark:text-white">
            Buy YouTube Videos
          </h2>
          <p class="text-base leading-relaxed">
            Williamsburg occupy sustainable snackwave gochujang. Pinterest cornhole brunch, slow-carb neutra irony.
          </p>
          <button
            :class="`flex mx-auto mt-6 text-white bg-${theme}-500 border-0 py-2 px-5 focus:outline-none hover:bg-${theme}-600 rounded`"
          >
            Button
          </button>
        </div>
        <div class="mb-10 px-4 sm:w-1/2">
          <div class="h-64 overflow-hidden rounded-lg">
            <img alt="content" class="h-full w-full object-cover object-center" src="https://dummyimage.com/1202x502">
          </div>
          <h2 class="title-font mb-3 mt-6 text-2xl font-medium text-gray-900 dark:text-white">
            The Catalyzer
          </h2>
          <p class="text-base leading-relaxed">
            Williamsburg occupy sustainable snackwave gochujang. Pinterest cornhole brunch, slow-carb neutra irony.
          </p>
          <button
            :class="`flex mx-auto mt-6 text-white bg-${theme}-500 border-0 py-2 px-5 focus:outline-none hover:bg-${theme}-600 rounded`"
          >
            Button
          </button>
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
