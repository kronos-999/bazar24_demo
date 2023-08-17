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
      <h2 class="title-font mb-2 text-2xl font-medium text-gray-900 md:w-2/5 sm:text-3xl dark:text-white">
        Kickstarter Actually Pinterest Brunch Bitters Occupy
      </h2>
      <div class="md:w-3/5 md:pl-6">
        <p class="text-base leading-relaxed">
          Taxidermy bushwick celiac master cleanse microdosing seitan. Fashion axe four dollar toast truffaut, direct
          trade kombucha brunch williamsburg keffiyeh gastropub tousled squid meh taiyaki drinking vinegar tacos.
        </p>
        <div class="mt-6 flex md:mt-4">
          <button
            :class="`inline-flex text-white bg-${theme}-500 border-0 py-1 px-4 focus:outline-none hover:bg-${theme}-600 rounded`"
          >
            Button
          </button>
          <a :class="`text-${theme}-500 inline-flex items-center ml-4 dark:text-${theme}-400`">Learn More
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
