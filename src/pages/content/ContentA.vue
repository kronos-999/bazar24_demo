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
      <div class="mb-20 w-full flex flex-col text-center">
        <h2 :class="`text-xs text-${theme}-500 tracking-widest font-medium title-font mb-1 dark:text-${theme}-400`">
          ROOF PARTY POLAROID
        </h2>
        <h1 class="title-font mb-4 text-2xl font-medium text-gray-900 sm:text-3xl dark:text-white">
          Master Cleanse Reliac Heirloom
        </h1>
        <p class="mx-auto text-base leading-relaxed lg:w-2/3">
          Whatever cardigan tote bag tumblr hexagon brooklyn asymmetrical gentrify, subway tile poke farm-to-table.
          Franzen you probably haven't heard of them man bun deep jianbing selfies heirloom prism food truck ugh squid
          celiac humblebrag.
        </p>
      </div>
      <div class="flex flex-wrap">
        <div
          class="border-l-2 border-gray-200 border-opacity-60 px-8 py-6 lg:w-1/2 md:w-full xl:w-1/4 dark:border-gray-800"
        >
          <h2 class="title-font mb-2 text-lg font-medium text-gray-900 sm:text-xl dark:text-white">
            Shooting Stars
          </h2>
          <p class="mb-4 text-base leading-relaxed">
            Fingerstache flexitarian street art 8-bit waistcoat. Distillery hexagon disrupt edison bulbche.
          </p>
          <a :class="`text-${theme}-500 inline-flex items-center dark:text-${theme}-400`">Learn More
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              class="ml-2 h-4 w-4" viewBox="0 0 24 24"
            >
              <path d="M5 12h14M12 5l7 7-7 7" />
            </svg>
          </a>
        </div>
        <div
          class="border-l-2 border-gray-200 border-opacity-60 px-8 py-6 lg:w-1/2 md:w-full xl:w-1/4 dark:border-gray-800"
        >
          <h2 class="title-font mb-2 text-lg font-medium text-gray-900 sm:text-xl dark:text-white">
            The Catalyzer
          </h2>
          <p class="mb-4 text-base leading-relaxed">
            Fingerstache flexitarian street art 8-bit waistcoat. Distillery hexagon disrupt edison bulbche.
          </p>
          <a :class="`text-${theme}-500 inline-flex items-center dark:text-${theme}-400`">Learn More
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              class="ml-2 h-4 w-4" viewBox="0 0 24 24"
            >
              <path d="M5 12h14M12 5l7 7-7 7" />
            </svg>
          </a>
        </div>
        <div
          class="border-l-2 border-gray-200 border-opacity-60 px-8 py-6 lg:w-1/2 md:w-full xl:w-1/4 dark:border-gray-800"
        >
          <h2 class="title-font mb-2 text-lg font-medium text-gray-900 sm:text-xl dark:text-white">
            Neptune
          </h2>
          <p class="mb-4 text-base leading-relaxed">
            Fingerstache flexitarian street art 8-bit waistcoat. Distillery hexagon disrupt edison bulbche.
          </p>
          <a :class="`text-${theme}-500 inline-flex items-center dark:text-${theme}-400`">Learn More
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              class="ml-2 h-4 w-4" viewBox="0 0 24 24"
            >
              <path d="M5 12h14M12 5l7 7-7 7" />
            </svg>
          </a>
        </div>
        <div
          class="border-l-2 border-gray-200 border-opacity-60 px-8 py-6 lg:w-1/2 md:w-full xl:w-1/4 dark:border-gray-800"
        >
          <h2 class="title-font mb-2 text-lg font-medium text-gray-900 sm:text-xl dark:text-white">
            Melanchole
          </h2>
          <p class="mb-4 text-base leading-relaxed">
            Fingerstache flexitarian street art 8-bit waistcoat. Distillery hexagon disrupt edison bulbche.
          </p>
          <a :class="`text-${theme}-500 inline-flex items-center dark:text-${theme}-400`">Learn More
            <svg
              fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              class="ml-2 h-4 w-4" viewBox="0 0 24 24"
            >
              <path d="M5 12h14M12 5l7 7-7 7" />
            </svg>
          </a>
        </div>
      </div>
      <button
        :class="`flex mx-auto mt-16 text-white bg-${theme}-500 border-0 py-2 px-8 focus:outline-none hover:bg-${theme}-600 rounded text-lg`"
      >
        Button
      </button>
    </div>
  </section>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>

<style></style>
