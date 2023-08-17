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
      <div class="mx-auto lg:w-2/3">
        <div class="relative mb-4 w-full flex flex-wrap bg-gray-100 px-10 py-32 dark:bg-gray-800">
          <img
            alt="gallery" class="absolute inset-0 block h-full w-full object-cover object-center opacity-25"
            src="https://dummyimage.com/820x340"
          >
          <div class="relative z-10 w-full text-center">
            <h2 class="title-font mb-2 text-2xl font-medium text-gray-900 dark:text-white">
              Shooting Stars
            </h2>
            <p class="leading-relaxed">
              Skateboard +1 mustache fixie paleo lumbersexual.
            </p>
            <a :class="`mt-3 text-${theme}-500 inline-flex items-center dark:text-${theme}-300`">Learn More
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                class="ml-2 h-4 w-4" viewBox="0 0 24 24"
              >
                <path d="M5 12h14M12 5l7 7-7 7" />
              </svg>
            </a>
          </div>
        </div>
        <div class="flex flex-wrap -mx-2">
          <div class="w-1/2 px-2">
            <div class="relative w-full flex flex-wrap bg-gray-100 px-6 py-16 dark:bg-gray-800 sm:px-10 sm:py-24">
              <img
                alt="gallery" class="absolute inset-0 block h-full w-full object-cover object-center opacity-25"
                src="https://dummyimage.com/542x460"
              >
              <div class="relative z-10 w-full text-center">
                <h2 class="title-font mb-2 text-xl font-medium text-gray-900 dark:text-white">
                  Shooting Stars
                </h2>
                <p class="leading-relaxed">
                  Skateboard +1 mustache fixie paleo lumbersexual.
                </p>
                <a :class="`mt-3 text-${theme}-500 inline-flex items-center dark:text-${theme}-300`">Learn More
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
          <div class="w-1/2 px-2">
            <div class="relative w-full flex flex-wrap bg-gray-100 px-6 py-16 dark:bg-gray-800 sm:px-10 sm:py-24">
              <img
                alt="gallery" class="absolute inset-0 block h-full w-full object-cover object-center opacity-25"
                src="https://dummyimage.com/542x420"
              >
              <div class="relative z-10 w-full text-center">
                <h2 class="title-font mb-2 text-xl font-medium text-gray-900 dark:text-white">
                  Shooting Stars
                </h2>
                <p class="leading-relaxed">
                  Skateboard +1 mustache fixie paleo lumbersexual.
                </p>
                <a :class="`mt-3 text-${theme}-500 inline-flex items-center dark:text-${theme}-300`">Learn More
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
      </div>
    </div>
  </section>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>

<style></style>
