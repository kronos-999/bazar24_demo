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
      <div class="w-full flex flex-wrap">
        <div class="lg:w-2/5 md:w-1/2 md:py-6 md:pr-10">
          <div class="relative flex pb-12">
            <div class="absolute inset-0 h-full w-10 flex items-center justify-center">
              <div class="pointer-events-none h-full w-1 bg-gray-200 dark:bg-gray-800" />
            </div>
            <div
              :class="`flex-shrink-0 w-10 h-10 rounded-full bg-${theme}-500 inline-flex items-center justify-center text-white relative z-10`"
            >
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                class="h-5 w-5" viewBox="0 0 24 24"
              >
                <path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z" />
              </svg>
            </div>
            <div class="flex-grow pl-4">
              <h2 class="title-font mb-1 text-sm font-medium tracking-wider text-gray-900 dark:text-white">
                STEP 1
              </h2>
              <p class="leading-relaxed">
                VHS cornhole pop-up, try-hard 8-bit iceland helvetica. Kinfolk bespoke try-hard cliche palo santo offal.
              </p>
            </div>
          </div>
          <div class="relative flex pb-12">
            <div class="absolute inset-0 h-full w-10 flex items-center justify-center">
              <div class="pointer-events-none h-full w-1 bg-gray-200 dark:bg-gray-800" />
            </div>
            <div
              :class="`flex-shrink-0 w-10 h-10 rounded-full bg-${theme}-500 inline-flex items-center justify-center text-white relative z-10`"
            >
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                class="h-5 w-5" viewBox="0 0 24 24"
              >
                <path d="M22 12h-4l-3 9L9 3l-3 9H2" />
              </svg>
            </div>
            <div class="flex-grow pl-4">
              <h2 class="title-font mb-1 text-sm font-medium tracking-wider text-gray-900 dark:text-white">
                STEP 2
              </h2>
              <p class="leading-relaxed">
                Vice migas literally kitsch +1 pok pok. Truffaut hot chicken slow-carb health goth, vape typewriter.
              </p>
            </div>
          </div>
          <div class="relative flex pb-12">
            <div class="absolute inset-0 h-full w-10 flex items-center justify-center">
              <div class="pointer-events-none h-full w-1 bg-gray-200 dark:bg-gray-800" />
            </div>
            <div
              :class="`flex-shrink-0 w-10 h-10 rounded-full bg-${theme}-500 inline-flex items-center justify-center text-white relative z-10`"
            >
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                class="h-5 w-5" viewBox="0 0 24 24"
              >
                <circle cx="12" cy="5" r="3" />
                <path d="M12 22V8M5 12H2a10 10 0 0020 0h-3" />
              </svg>
            </div>
            <div class="flex-grow pl-4">
              <h2 class="title-font mb-1 text-sm font-medium tracking-wider text-gray-900 dark:text-white">
                STEP 3
              </h2>
              <p class="leading-relaxed">
                Coloring book nar whal glossier master cleanse umami. Salvia +1 master cleanse blog taiyaki.
              </p>
            </div>
          </div>
          <div class="relative flex pb-12">
            <div class="absolute inset-0 h-full w-10 flex items-center justify-center">
              <div class="pointer-events-none h-full w-1 bg-gray-200 dark:bg-gray-800" />
            </div>
            <div
              :class="`flex-shrink-0 w-10 h-10 rounded-full bg-${theme}-500 inline-flex items-center justify-center text-white relative z-10`"
            >
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                class="h-5 w-5" viewBox="0 0 24 24"
              >
                <path d="M20 21v-2a4 4 0 00-4-4H8a4 4 0 00-4 4v2" />
                <circle cx="12" cy="7" r="4" />
              </svg>
            </div>
            <div class="flex-grow pl-4">
              <h2 class="title-font mb-1 text-sm font-medium tracking-wider text-gray-900 dark:text-white">
                STEP 4
              </h2>
              <p class="leading-relaxed">
                VHS cornhole pop-up, try-hard 8-bit iceland helvetica. Kinfolk bespoke try-hard cliche palo santo offal.
              </p>
            </div>
          </div>
          <div class="relative flex">
            <div
              :class="`flex-shrink-0 w-10 h-10 rounded-full bg-${theme}-500 inline-flex items-center justify-center text-white relative z-10`"
            >
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                class="h-5 w-5" viewBox="0 0 24 24"
              >
                <path d="M22 11.08V12a10 10 0 11-5.93-9.14" />
                <path d="M22 4L12 14.01l-3-3" />
              </svg>
            </div>
            <div class="flex-grow pl-4">
              <h2 class="title-font mb-1 text-sm font-medium tracking-wider text-gray-900 dark:text-white">
                FINISH
              </h2>
              <p class="leading-relaxed">
                Pitchfork ugh tattooed scenester echo park gastropub whatever cold-pressed retro.
              </p>
            </div>
          </div>
        </div>
        <img
          class="mt-12 rounded-lg object-cover object-center md:mt-0 lg:w-3/5 md:w-1/2"
          src="https://dummyimage.com/1200x500" alt="step"
        >
      </div>
    </div>
  </section>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>

<style></style>
