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
    <div class="mx-auto px-5 py-24 container">
      <div class="mb-12 w-full flex flex-col text-center">
        <h1 class="title-font mb-4 text-2xl font-medium text-gray-900 sm:text-3xl dark:text-white">
          Contact Us
        </h1>
        <p class="mx-auto text-base leading-relaxed lg:w-2/3">
          Whatever cardigan tote bag tumblr hexagon brooklyn asymmetrical gentrify.
        </p>
      </div>
      <div class="mx-auto lg:w-1/2 md:w-2/3">
        <div class="flex flex-wrap -m-2">
          <div class="w-1/2 p-2">
            <div class="relative">
              <label for="name" class="text-sm leading-7 text-gray-600 dark:text-gray-400">Name</label>
              <input
                id="name" type="text" name="name"
                :class="`w-full bg-gray-100 bg-opacity-50 rounded border border-gray-300 focus:border-${theme}-500 focus:bg-white focus:ring-2 focus:ring-${theme}-200 text-base outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out dark:bg-gray-800 dark:bg-opacity-40 dark:border-gray-700 dark:focus:bg-gray-900 dark:focus:ring-${theme}-900 dark:text-gray-100`"
              >
            </div>
          </div>
          <div class="w-1/2 p-2">
            <div class="relative">
              <label for="email" class="text-sm leading-7 text-gray-600 dark:text-gray-400">Email</label>
              <input
                id="email" type="email" name="email"
                :class="`w-full bg-gray-100 bg-opacity-50 rounded border border-gray-300 focus:border-${theme}-500 focus:bg-white focus:ring-2 focus:ring-${theme}-200 text-base outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out dark:bg-gray-800 dark:bg-opacity-40 dark:border-gray-700 dark:focus:bg-gray-900 dark:focus:ring-${theme}-900 dark:text-gray-100`"
              >
            </div>
          </div>
          <div class="w-full p-2">
            <div class="relative">
              <label for="message" class="text-sm leading-7 text-gray-600 dark:text-gray-400">Message</label>
              <textarea
                id="message" name="message"
                :class="`w-full bg-gray-100 bg-opacity-50 rounded border border-gray-300 focus:border-${theme}-500 focus:bg-white focus:ring-2 focus:ring-${theme}-200 h-32 text-base outline-none text-gray-700 py-1 px-3 resize-none leading-6 transition-colors duration-200 ease-in-out dark:bg-gray-800 dark:bg-opacity-40 dark:border-gray-700 dark:focus:bg-gray-900 dark:focus:ring-${theme}-900 dark:text-gray-100`"
              />
            </div>
          </div>
          <div class="w-full p-2">
            <button
              :class="`flex mx-auto text-white bg-${theme}-500 border-0 py-2 px-8 focus:outline-none hover:bg-${theme}-600 rounded text-lg`"
            >
              Button
            </button>
          </div>
          <div class="mt-8 w-full border-t border-gray-200 p-2 pt-8 text-center dark:border-gray-800">
            <a :class="`text-${theme}-500 dark:text-${theme}-400`">example@email.com</a>
            <p class="my-5 leading-normal">
              49 Smith St. <br>Saint Cloud, MN 56301
            </p>
            <span class="inline-flex">
              <a class="text-gray-500">
                <svg
                  fill="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" class="h-5 w-5"
                  viewBox="0 0 24 24"
                >
                  <path d="M18 2h-3a5 5 0 00-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 011-1h3z" />
                </svg>
              </a>
              <a class="ml-4 text-gray-500">
                <svg
                  fill="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" class="h-5 w-5"
                  viewBox="0 0 24 24"
                >
                  <path
                    d="M23 3a10.9 10.9 0 01-3.14 1.53 4.48 4.48 0 00-7.86 3v1A10.66 10.66 0 013 4s-4 9 5 13a11.64 11.64 0 01-7 2c9 5 20 0 20-11.5a4.5 4.5 0 00-.08-.83A7.72 7.72 0 0023 3z"
                  />
                </svg>
              </a>
              <a class="ml-4 text-gray-500">
                <svg
                  fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  class="h-5 w-5" viewBox="0 0 24 24"
                >
                  <rect width="20" height="20" x="2" y="2" rx="5" ry="5" />
                  <path d="M16 11.37A4 4 0 1112.63 8 4 4 0 0116 11.37zm1.5-4.87h.01" />
                </svg>
              </a>
              <a class="ml-4 text-gray-500">
                <svg
                  fill="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" class="h-5 w-5"
                  viewBox="0 0 24 24"
                >
                  <path
                    d="M21 11.5a8.38 8.38 0 01-.9 3.8 8.5 8.5 0 01-7.6 4.7 8.38 8.38 0 01-3.8-.9L3 21l1.9-5.7a8.38 8.38 0 01-.9-3.8 8.5 8.5 0 014.7-7.6 8.38 8.38 0 013.8-.9h.5a8.48 8.48 0 018 8v.5z"
                  />
                </svg>
              </a>
            </span>
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
