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
      <div class="flex flex-wrap -m-4">
        <div class="mb-6 p-4 lg:mb-0 lg:w-1/3">
          <div class="h-full text-center">
            <img
              alt="testimonial"
              class="mb-8 inline-block h-20 w-20 border-2 border-gray-200 rounded-full bg-gray-100 object-cover object-center dark:border-gray-800 dark:bg-gray-800 dark:bg-opacity-10"
              src="https://dummyimage.com/302x302"
            >
            <p class="leading-relaxed">
              Edison bulb retro cloud bread echo park, helvetica stumptown taiyaki taxidermy 90's cronut +1 kinfolk.
              Single-origin coffee ennui shaman taiyaki vape DIY tote bag drinking vinegar cronut adaptogen squid fanny
              pack vaporware.
            </p>
            <span :class="`inline-block h-1 w-10 rounded bg-${theme}-500 mt-6 mb-4`" />
            <h2 class="title-font text-sm font-medium tracking-wider text-gray-900 dark:text-white">
              HOLDEN CAULFIELD
            </h2>
            <p class="text-gray-500">
              Senior Product Designer
            </p>
          </div>
        </div>
        <div class="mb-6 p-4 lg:mb-0 lg:w-1/3">
          <div class="h-full text-center">
            <img
              alt="testimonial"
              class="mb-8 inline-block h-20 w-20 border-2 border-gray-200 rounded-full bg-gray-100 object-cover object-center dark:border-gray-800 dark:bg-gray-800 dark:bg-opacity-10"
              src="https://dummyimage.com/300x300"
            >
            <p class="leading-relaxed">
              Edison bulb retro cloud bread echo park, helvetica stumptown taiyaki taxidermy 90's cronut +1 kinfolk.
              Single-origin coffee ennui shaman taiyaki vape DIY tote bag drinking vinegar cronut adaptogen squid fanny
              pack vaporware.
            </p>
            <span :class="`inline-block h-1 w-10 rounded bg-${theme}-500 mt-6 mb-4`" />
            <h2 class="title-font text-sm font-medium tracking-wider text-gray-900 dark:text-white">
              ALPER KAMU
            </h2>
            <p class="text-gray-500">
              UI Develeoper
            </p>
          </div>
        </div>
        <div class="p-4 lg:mb-0 lg:w-1/3">
          <div class="h-full text-center">
            <img
              alt="testimonial"
              class="mb-8 inline-block h-20 w-20 border-2 border-gray-200 rounded-full bg-gray-100 object-cover object-center dark:border-gray-800 dark:bg-gray-800 dark:bg-opacity-10"
              src="https://dummyimage.com/305x305"
            >
            <p class="leading-relaxed">
              Edison bulb retro cloud bread echo park, helvetica stumptown taiyaki taxidermy 90's cronut +1 kinfolk.
              Single-origin coffee ennui shaman taiyaki vape DIY tote bag drinking vinegar cronut adaptogen squid fanny
              pack vaporware.
            </p>
            <span :class="`inline-block h-1 w-10 rounded bg-${theme}-500 mt-6 mb-4`" />
            <h2 class="title-font text-sm font-medium tracking-wider text-gray-900 dark:text-white">
              HENRY LETHAM
            </h2>
            <p class="text-gray-500">
              CTO
            </p>
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
