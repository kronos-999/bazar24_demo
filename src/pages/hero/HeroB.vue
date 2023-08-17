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
    <div class="mx-auto flex flex-col items-center justify-center px-5 py-24 container">
      <img
        class="mb-10 w-5/6 rounded object-cover object-center lg:w-2/6 md:w-3/6" alt="hero"
        src="https://dummyimage.com/720x600"
      >
      <div class="w-full text-center lg:w-2/3">
        <h1 class="title-font mb-4 text-3xl font-medium text-gray-900 sm:text-4xl dark:text-white">
          Microdosing synth tattooed vexillologist
        </h1>
        <p class="mb-8 leading-relaxed">
          Meggings kinfolk echo park stumptown DIY, kale chips beard jianbing tousled. Chambray dreamcatcher trust fund,
          kitsch vice godard disrupt ramps hexagon mustache umami snackwave tilde chillwave ugh. Pour-over meditation
          PBR&B pickled ennui celiac mlkshk freegan photo booth af fingerstache pitchfork.
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
