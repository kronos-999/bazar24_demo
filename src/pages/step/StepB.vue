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
    <div class="mx-auto flex flex-col flex-wrap px-5 py-24 container">
      <div class="mx-auto mb-20 flex flex-wrap">
        <a
          :class="`sm:px-6 py-3 w-1/2 sm:w-auto justify-center sm:justify-start border-b-2 title-font font-medium bg-gray-100 inline-flex items-center leading-none border-${theme}-500 text-${theme}-500 tracking-wider rounded-t dark:bg-gray-800 dark:text-white`"
        >
          <svg
            fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
            class="mr-3 h-5 w-5" viewBox="0 0 24 24"
          >
            <path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z" />
          </svg>STEP 1
        </a>
        <a
          class="title-font w-1/2 inline-flex items-center justify-center border-b-2 border-gray-200 py-3 font-medium leading-none tracking-wider sm:w-auto sm:justify-start dark:border-gray-800 sm:px-6 hover:text-gray-900 dark:hover:text-white"
        >
          <svg
            fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
            class="mr-3 h-5 w-5" viewBox="0 0 24 24"
          >
            <path d="M22 12h-4l-3 9L9 3l-3 9H2" />
          </svg>STEP 2
        </a>
        <a
          class="title-font w-1/2 inline-flex items-center justify-center border-b-2 border-gray-200 py-3 font-medium leading-none tracking-wider sm:w-auto sm:justify-start dark:border-gray-800 sm:px-6 hover:text-gray-900 dark:hover:text-white"
        >
          <svg
            fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
            class="mr-3 h-5 w-5" viewBox="0 0 24 24"
          >
            <circle cx="12" cy="5" r="3" />
            <path d="M12 22V8M5 12H2a10 10 0 0020 0h-3" />
          </svg>STEP 3
        </a>
        <a
          class="title-font w-1/2 inline-flex items-center justify-center border-b-2 border-gray-200 py-3 font-medium leading-none tracking-wider sm:w-auto sm:justify-start dark:border-gray-800 sm:px-6 hover:text-gray-900 dark:hover:text-white"
        >
          <svg
            fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
            class="mr-3 h-5 w-5" viewBox="0 0 24 24"
          >
            <path d="M20 21v-2a4 4 0 00-4-4H8a4 4 0 00-4 4v2" />
            <circle cx="12" cy="7" r="4" />
          </svg>STEP 4
        </a>
      </div>
      <img
        class="mx-auto mb-10 block w-2/3 rounded object-cover object-center lg:w-1/3 md:w-1/2 xl:w-1/4" alt="hero"
        src="https://dummyimage.com/720x600"
      >
      <div class="w-full flex flex-col text-center">
        <h1 class="title-font mb-4 text-xl font-medium text-gray-900 dark:text-white">
          Master Cleanse Reliac Heirloom
        </h1>
        <p class="mx-auto text-base leading-relaxed lg:w-2/3">
          Whatever cardigan tote bag tumblr hexagon brooklyn asymmetrical gentrify, subway tile poke farm-to-table.
          Franzen you probably haven't heard of them man bun deep jianbing selfies heirloom prism food truck ugh squid
          celiac humblebrag.
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
