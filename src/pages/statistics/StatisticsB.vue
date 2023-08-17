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
    <div class="mx-auto flex flex-wrap px-5 py-24 container">
      <div class="mb-auto mt-auto flex flex-wrap content-start -mx-4 lg:w-1/2 sm:w-2/3 sm:pr-10">
        <div class="mb-6 w-full px-4 sm:p-4">
          <h1 class="title-font mb-2 text-xl font-medium text-gray-900 dark:text-white">
            Moon hashtag pop-up try-hard offal truffaut
          </h1>
          <div class="leading-relaxed">
            Pour-over craft beer pug drinking vinegar live-edge gastropub, keytar neutra sustainable fingerstache
            kickstarter.
          </div>
        </div>
        <div class="w-1/2 p-4 lg:w-1/4 sm:w-1/2">
          <h2 class="title-font text-3xl font-medium text-gray-900 dark:text-white">
            2.7K
          </h2>
          <p class="leading-relaxed">
            Users
          </p>
        </div>
        <div class="w-1/2 p-4 lg:w-1/4 sm:w-1/2">
          <h2 class="title-font text-3xl font-medium text-gray-900 dark:text-white">
            1.8K
          </h2>
          <p class="leading-relaxed">
            Subscribes
          </p>
        </div>
        <div class="w-1/2 p-4 lg:w-1/4 sm:w-1/2">
          <h2 class="title-font text-3xl font-medium text-gray-900 dark:text-white">
            35
          </h2>
          <p class="leading-relaxed">
            Downloads
          </p>
        </div>
        <div class="w-1/2 p-4 lg:w-1/4 sm:w-1/2">
          <h2 class="title-font text-3xl font-medium text-gray-900 dark:text-white">
            4
          </h2>
          <p class="leading-relaxed">
            Products
          </p>
        </div>
      </div>
      <div class="mt-6 w-full overflow-hidden rounded-lg sm:mt-0 lg:w-1/2 sm:w-1/3">
        <img class="h-full w-full object-cover object-center" src="https://dummyimage.com/600x300" alt="stats">
      </div>
    </div>
  </section>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>

<style></style>
