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
      <div class="mb-20 w-full flex flex-wrap">
        <h1 class="title-font mb-4 text-2xl font-medium text-gray-900 lg:mb-0 lg:w-1/3 sm:text-3xl dark:text-white">
          Master Cleanse Reliac Heirloom
        </h1>
        <p class="mx-auto text-base leading-relaxed lg:w-2/3 lg:pl-6">
          Whatever cardigan tote bag tumblr hexagon brooklyn asymmetrical gentrify, subway tile poke farm-to-table.
          Franzen you probably haven't heard of them man bun deep jianbing selfies heirloom.
        </p>
      </div>
      <div class="flex flex-wrap -m-1 md:-m-2">
        <div class="w-1/2 flex flex-wrap">
          <div class="w-1/2 p-1 md:p-2">
            <img
              alt="gallery" class="block h-full w-full object-cover object-center"
              src="https://dummyimage.com/500x300"
            >
          </div>
          <div class="w-1/2 p-1 md:p-2">
            <img
              alt="gallery" class="block h-full w-full object-cover object-center"
              src="https://dummyimage.com/501x301"
            >
          </div>
          <div class="w-full p-1 md:p-2">
            <img
              alt="gallery" class="block h-full w-full object-cover object-center"
              src="https://dummyimage.com/600x360"
            >
          </div>
        </div>
        <div class="w-1/2 flex flex-wrap">
          <div class="w-full p-1 md:p-2">
            <img
              alt="gallery" class="block h-full w-full object-cover object-center"
              src="https://dummyimage.com/601x361"
            >
          </div>
          <div class="w-1/2 p-1 md:p-2">
            <img
              alt="gallery" class="block h-full w-full object-cover object-center"
              src="https://dummyimage.com/502x302"
            >
          </div>
          <div class="w-1/2 p-1 md:p-2">
            <img
              alt="gallery" class="block h-full w-full object-cover object-center"
              src="https://dummyimage.com/503x303"
            >
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
