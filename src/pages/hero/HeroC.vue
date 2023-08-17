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
    <div class="mx-auto flex flex-col items-center px-5 py-24 container md:flex-row">
      <div class="mb-10 w-5/6 md:mb-0 lg:max-w-lg lg:w-full md:w-1/2">
        <img class="rounded object-cover object-center" alt="hero" src="https://dummyimage.com/720x600">
      </div>
      <div
        class="flex flex-col items-center text-center md:w-1/2 lg:flex-grow md:items-start lg:pl-24 md:pl-16 md:text-left"
      >
        <h1 class="title-font mb-4 text-3xl font-medium text-gray-900 sm:text-4xl dark:text-white">
          Before they sold out <br class="hidden lg:inline-block">readymade gluten
        </h1>
        <p class="mb-8 leading-relaxed">
          Copper mug try-hard pitchfork pour-over freegan heirloom neutra air plant cold-pressed tacos poke beard tote
          bag. Heirloom echo park mlkshk tote bag selvage hot chicken authentic tumeric truffaut hexagon try-hard
          chambray.
        </p>
        <div class="flex justify-center">
          <button
            :class="`inline-flex text-white bg-${theme}-500 border-0 py-2 px-6 focus:outline-none hover:bg-${theme}-600 rounded text-lg`"
          >
            Button
          </button>
          <button
            class="ml-4 inline-flex border-0 rounded bg-gray-100 px-6 py-2 text-lg text-gray-700 dark:bg-gray-800 hover:bg-gray-200 dark:text-gray-400 focus:outline-none dark:hover:bg-gray-700 dark:hover:text-white"
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
