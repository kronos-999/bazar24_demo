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
      <div class="flex flex-wrap text-center -m-4">
        <div class="w-1/2 p-4 sm:w-1/4">
          <h2 class="title-font text-3xl font-medium text-gray-900 sm:text-4xl dark:text-white">
            2.7K
          </h2>
          <p class="leading-relaxed">
            Users
          </p>
        </div>
        <div class="w-1/2 p-4 sm:w-1/4">
          <h2 class="title-font text-3xl font-medium text-gray-900 sm:text-4xl dark:text-white">
            1.8K
          </h2>
          <p class="leading-relaxed">
            Subscribes
          </p>
        </div>
        <div class="w-1/2 p-4 sm:w-1/4">
          <h2 class="title-font text-3xl font-medium text-gray-900 sm:text-4xl dark:text-white">
            35
          </h2>
          <p class="leading-relaxed">
            Downloads
          </p>
        </div>
        <div class="w-1/2 p-4 sm:w-1/4">
          <h2 class="title-font text-3xl font-medium text-gray-900 sm:text-4xl dark:text-white">
            4
          </h2>
          <p class="leading-relaxed">
            Products
          </p>
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
