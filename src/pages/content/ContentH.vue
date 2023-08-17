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
      <div class="flex flex-col">
        <div class="h-1 overflow-hidden rounded bg-gray-200 dark:bg-gray-800">
          <div :class="`w-24 h-full bg-${theme}-500`" />
        </div>
        <div class="mb-12 flex flex-col flex-wrap py-6 sm:flex-row">
          <h1 class="title-font mb-2 text-2xl font-medium text-gray-900 sm:mb-0 sm:w-2/5 dark:text-white">
            Space The Final Frontier
          </h1>
          <p class="pl-0 text-base leading-relaxed sm:w-3/5 sm:pl-10">
            Street art subway tile salvia four dollar toast bitters selfies quinoa yuccie synth meditation iPhone
            intelligentsia prism tofu. Viral gochujang bitters dreamcatcher.
          </p>
        </div>
      </div>
      <div class="flex flex-wrap -mx-4 -mb-10 -mt-4 sm:-m-4">
        <div class="mb-6 p-4 sm:mb-0 md:w-1/3">
          <div class="h-64 overflow-hidden rounded-lg">
            <img alt="content" class="h-full w-full object-cover object-center" src="https://dummyimage.com/1203x503">
          </div>
          <h2 class="title-font mt-5 text-xl font-medium text-gray-900 dark:text-white">
            Shooting Stars
          </h2>
          <p class="mt-2 text-base leading-relaxed">
            Swag shoivdigoitch literally meditation subway tile tumblr cold-pressed. Gastropub street art beard
            dreamcatcher neutra, ethical XOXO lumbersexual.
          </p>
          <a :class="`text-${theme}-500 inline-flex items-center mt-3 dark:text-${theme}-400`">Learn More
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              class="ml-2 h-4 w-4" viewBox="0 0 24 24"
            >
              <path d="M5 12h14M12 5l7 7-7 7" />
            </svg>
          </a>
        </div>
        <div class="mb-6 p-4 sm:mb-0 md:w-1/3">
          <div class="h-64 overflow-hidden rounded-lg">
            <img alt="content" class="h-full w-full object-cover object-center" src="https://dummyimage.com/1204x504">
          </div>
          <h2 class="title-font mt-5 text-xl font-medium text-gray-900 dark:text-white">
            The Catalyzer
          </h2>
          <p class="mt-2 text-base leading-relaxed">
            Swag shoivdigoitch literally meditation subway tile tumblr cold-pressed. Gastropub street art beard
            dreamcatcher neutra, ethical XOXO lumbersexual.
          </p>
          <a :class="`text-${theme}-500 inline-flex items-center mt-3 dark:text-${theme}-400`">Learn More
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              class="ml-2 h-4 w-4" viewBox="0 0 24 24"
            >
              <path d="M5 12h14M12 5l7 7-7 7" />
            </svg>
          </a>
        </div>
        <div class="mb-6 p-4 sm:mb-0 md:w-1/3">
          <div class="h-64 overflow-hidden rounded-lg">
            <img alt="content" class="h-full w-full object-cover object-center" src="https://dummyimage.com/1205x505">
          </div>
          <h2 class="title-font mt-5 text-xl font-medium text-gray-900 dark:text-white">
            The 400 Blows
          </h2>
          <p class="mt-2 text-base leading-relaxed">
            Swag shoivdigoitch literally meditation subway tile tumblr cold-pressed. Gastropub street art beard
            dreamcatcher neutra, ethical XOXO lumbersexual.
          </p>
          <a :class="`text-${theme}-500 inline-flex items-center mt-3 dark:text-${theme}-400`">Learn More
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              class="ml-2 h-4 w-4" viewBox="0 0 24 24"
            >
              <path d="M5 12h14M12 5l7 7-7 7" />
            </svg>
          </a>
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
