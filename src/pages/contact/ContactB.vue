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
  <section class="body-font relative text-gray-600 dark:bg-gray-900 dark:text-gray-400">
    <div class="mx-auto flex flex-wrap px-5 py-24 container sm:flex-nowrap">
      <div
        class="relative flex items-end justify-start overflow-hidden rounded-lg bg-gray-300 p-10 sm:mr-10 lg:w-2/3 md:w-1/2 dark:bg-gray-900"
      >
        <iframe
          width="100%" height="100%" class="absolute inset-0" frameborder="0" title="map" marginheight="0"
          marginwidth="0" scrolling="no"
          src="https://maps.google.com/maps?width=100%&height=600&hl=en&q=%C4%B0zmir+(My%20Business%20Name)&ie=UTF8&t=&z=14&iwloc=B&output=embed"
          style="filter: grayscale(1) contrast(1.2) opacity(0.4)"
        />
        <div class="relative flex flex-wrap rounded bg-white py-6 shadow-md dark:bg-gray-900">
          <div class="px-6 lg:w-1/2">
            <h2 class="title-font text-xs font-semibold tracking-widest text-gray-900 dark:text-white">
              ADDRESS
            </h2>
            <p class="mt-1">
              Photo booth tattooed prism, portland taiyaki hoodie neutra typewriter
            </p>
          </div>
          <div class="mt-4 px-6 lg:mt-0 lg:w-1/2">
            <h2 class="title-font text-xs font-semibold tracking-widest text-gray-900 dark:text-white">
              EMAIL
            </h2>
            <a :class="`text-${theme}-500 leading-relaxed dark:text-${theme}-400`">example@email.com</a>
            <h2 class="title-font mt-4 text-xs font-semibold tracking-widest text-gray-900 dark:text-white">
              PHONE
            </h2>
            <p class="leading-relaxed">
              123-456-7890
            </p>
          </div>
        </div>
      </div>
      <div class="mt-8 w-full flex flex-col bg-white md:ml-auto md:mt-0 lg:w-1/3 md:w-1/2 md:py-8">
        <h2 class="title-font mb-1 text-lg font-medium text-gray-900 dark:text-white">
          Feedback
        </h2>
        <p class="mb-5 leading-relaxed text-gray-600">
          Post-ironic portland shabby chic echo park, banjo fashion axe
        </p>
        <div class="relative mb-4">
          <label for="name" class="text-sm leading-7 text-gray-600 dark:text-gray-400">Name</label>
          <input
            id="name" type="text" name="name"
            :class="`w-full bg-white rounded border border-gray-300 focus:border-${theme}-500 focus:ring-2 focus:ring-${theme}-200 text-base outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out dark:bg-gray-800 dark:border-gray-700 dark:focus:ring-${theme}-900 dark:text-gray-100`"
          >
        </div>
        <div class="relative mb-4">
          <label for="email" class="text-sm leading-7 text-gray-600 dark:text-gray-400">Email</label>
          <input
            id="email" type="email" name="email"
            :class="`w-full bg-white rounded border border-gray-300 focus:border-${theme}-500 focus:ring-2 focus:ring-${theme}-200 text-base outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out dark:bg-gray-800 dark:border-gray-700 dark:focus:ring-${theme}-900 dark:text-gray-100`"
          >
        </div>
        <div class="relative mb-4">
          <label for="message" class="text-sm leading-7 text-gray-600 dark:text-gray-400">Message</label>
          <textarea
            id="message" name="message"
            :class="`w-full bg-white rounded border border-gray-300 focus:border-${theme}-500 focus:ring-2 focus:ring-${theme}-200 h-32 text-base outline-none text-gray-700 py-1 px-3 resize-none leading-6 transition-colors duration-200 ease-in-out dark:bg-gray-800 dark:border-gray-700 dark:focus:ring-${theme}-900 dark:text-gray-100`"
          />
        </div>
        <button
          :class="`text-white bg-${theme}-500 border-0 py-2 px-6 focus:outline-none hover:bg-${theme}-600 rounded text-lg`"
        >
          Button
        </button>
        <p class="mt-3 text-xs text-gray-500 dark:text-gray-400 dark:text-opacity-90">
          Chicharrones blog helvetica normcore iceland tousled brook viral artisan.
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
