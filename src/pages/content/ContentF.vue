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
    <div class="mx-auto flex flex-col px-5 py-24 container">
      <div class="mx-auto lg:w-4/6">
        <div class="h-64 overflow-hidden rounded-lg">
          <img alt="content" class="h-full w-full object-cover object-center" src="https://dummyimage.com/1200x500">
        </div>
        <div class="mt-10 flex flex-col sm:flex-row">
          <div class="text-center sm:w-1/3 sm:py-8 sm:pr-8">
            <div
              class="h-20 w-20 inline-flex items-center justify-center rounded-full bg-gray-200 text-gray-400 dark:bg-gray-800 dark:text-gray-600"
            >
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                class="h-10 w-10" viewBox="0 0 24 24"
              >
                <path d="M20 21v-2a4 4 0 00-4-4H8a4 4 0 00-4 4v2" />
                <circle cx="12" cy="7" r="4" />
              </svg>
            </div>
            <div class="flex flex-col items-center justify-center text-center">
              <h2 class="title-font mt-4 text-lg font-medium text-gray-900 dark:text-white">
                Phoebe Caulfield
              </h2>
              <div :class="`w-12 h-1 bg-${theme}-500 rounded mt-2 mb-4`" />
              <p class="text-base dark:text-gray-400">
                Raclette knausgaard hella meggs normcore williamsburg enamel pin sartorial venmo tbh hot chicken
                gentrify portland.
              </p>
            </div>
          </div>
          <div
            class="mt-4 border-t border-gray-200 pt-4 text-center sm:mt-0 sm:w-2/3 sm:border-l sm:border-t-0 dark:border-gray-800 sm:py-8 sm:pl-8 sm:text-left"
          >
            <p class="mb-4 text-lg leading-relaxed">
              Meggings portland fingerstache lyft, post-ironic fixie man bun banh mi umami everyday carry hexagon
              locavore direct trade art party. Locavore small batch listicle gastropub farm-to-table lumbersexual salvia
              messenger bag. Coloring book flannel truffaut craft beer drinking vinegar sartorial, disrupt fashion axe
              normcore meh butcher. Portland 90's scenester vexillologist forage post-ironic asymmetrical, chartreuse
              disrupt butcher paleo intelligentsia pabst before they sold out four loko. 3 wolf moon brooklyn.
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
      </div>
    </div>
  </section>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>

<style></style>
