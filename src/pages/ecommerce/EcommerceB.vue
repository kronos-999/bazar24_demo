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
  <section class="body-font overflow-hidden text-gray-600 dark:bg-gray-900 dark:text-gray-400">
    <div class="mx-auto px-5 py-24 container">
      <div class="mx-auto flex flex-wrap lg:w-4/5">
        <img
          alt="ecommerce" class="h-64 w-full rounded object-cover object-center lg:h-auto lg:w-1/2"
          src="https://dummyimage.com/400x400"
        >
        <div class="mt-6 w-full lg:mt-0 lg:w-1/2 lg:py-6 lg:pl-10">
          <h2 class="title-font text-sm tracking-widest text-gray-500">
            BRAND NAME
          </h2>
          <h1 class="title-font mb-1 text-3xl font-medium text-gray-900 dark:text-white">
            The Catcher in the Rye
          </h1>
          <div class="mb-4 flex">
            <span class="flex items-center">
              <svg
                fill="currentColor" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                stroke-width="2" :class="`w-4 h-4 text-${theme}-500 dark:text-${theme}-400`" viewBox="0 0 24 24"
              >
                <path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z" />
              </svg>
              <svg
                fill="currentColor" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                stroke-width="2" :class="`w-4 h-4 text-${theme}-500 dark:text-${theme}-400`" viewBox="0 0 24 24"
              >
                <path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z" />
              </svg>
              <svg
                fill="currentColor" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                stroke-width="2" :class="`w-4 h-4 text-${theme}-500 dark:text-${theme}-400`" viewBox="0 0 24 24"
              >
                <path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z" />
              </svg>
              <svg
                fill="currentColor" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round"
                stroke-width="2" :class="`w-4 h-4 text-${theme}-500 dark:text-${theme}-400`" viewBox="0 0 24 24"
              >
                <path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z" />
              </svg>
              <svg
                fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                :class="`w-4 h-4 text-${theme}-500 dark:text-${theme}-400`" viewBox="0 0 24 24"
              >
                <path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z" />
              </svg>
              <span class="ml-3 text-gray-600">4 Reviews</span>
            </span>
            <span
              class="space-x-2s ml-3 flex border-l-2 border-gray-200 py-2 pl-3 dark:border-gray-800 dark:text-gray-500 dark:space-x-2"
            >
              <a class="text-gray-500">
                <svg
                  fill="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" class="h-5 w-5"
                  viewBox="0 0 24 24"
                >
                  <path d="M18 2h-3a5 5 0 00-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 011-1h3z" />
                </svg>
              </a>
              <a class="text-gray-500">
                <svg
                  fill="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" class="h-5 w-5"
                  viewBox="0 0 24 24"
                >
                  <path
                    d="M23 3a10.9 10.9 0 01-3.14 1.53 4.48 4.48 0 00-7.86 3v1A10.66 10.66 0 013 4s-4 9 5 13a11.64 11.64 0 01-7 2c9 5 20 0 20-11.5a4.5 4.5 0 00-.08-.83A7.72 7.72 0 0023 3z"
                  />
                </svg>
              </a>
              <a class="text-gray-500">
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
          <p class="leading-relaxed">
            Fam locavore kickstarter distillery. Mixtape chillwave tumeric sriracha taximy chia microdosing tilde DIY.
            XOXO fam indxgo juiceramps cornhole raw denim forage brooklyn. Everyday carry +1 seitan poutine tumeric.
            Gastropub blue bottle austin listicle pour-over, neutra jean shorts keytar banjo tattooed umami cardigan.
          </p>
          <div class="mb-5 mt-6 flex items-center border-b-2 border-gray-100 pb-5 dark:border-gray-800">
            <div class="flex">
              <span class="mr-3">Color</span>
              <button
                class="h-6 w-6 border-2 border-gray-300 rounded-full dark:border-gray-800 focus:outline-none"
              />
              <button
                class="ml-1 h-6 w-6 border-2 border-gray-300 rounded-full bg-gray-700 dark:border-gray-800 focus:outline-none"
              />
              <button
                :class="`border-2 border-gray-300 ml-1 bg-${theme}-500 rounded-full w-6 h-6 focus:outline-none dark:border-gray-800`"
              />
            </div>
            <div class="ml-6 flex items-center">
              <span class="mr-3">Size</span>
              <div class="relative">
                <select
                  :class="`rounded border appearance-none border-gray-300 py-2 focus:outline-none focus:ring-2 focus:ring-${theme}-200 focus:border-${theme}-500 text-base pl-3 pr-10 dark:border-gray-700 dark:focus:ring-${theme}-900 dark:bg-transparent dark:text-white`"
                >
                  <option>SM</option>
                  <option>M</option>
                  <option>L</option>
                  <option>XL</option>
                </select>
                <span
                  class="pointer-events-none absolute right-0 top-0 h-full w-10 flex items-center justify-center text-center text-gray-600"
                >
                  <svg
                    fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    class="h-4 w-4" viewBox="0 0 24 24"
                  >
                    <path d="M6 9l6 6 6-6" />
                  </svg>
                </span>
              </div>
            </div>
          </div>
          <div class="flex">
            <span class="title-font text-2xl font-medium text-gray-900 dark:text-white">$58.00</span>
            <button
              :class="`flex ml-auto text-white bg-${theme}-500 border-0 py-2 px-6 focus:outline-none hover:bg-${theme}-600 rounded`"
            >
              Button
            </button>
            <button
              class="ml-4 h-10 w-10 inline-flex items-center justify-center border-0 rounded-full bg-gray-200 p-0 text-gray-500 dark:bg-gray-800"
            >
              <svg
                fill="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" class="h-5 w-5"
                viewBox="0 0 24 24"
              >
                <path
                  d="M20.84 4.61a5.5 5.5 0 00-7.78 0L12 5.67l-1.06-1.06a5.5 5.5 0 00-7.78 7.78l1.06 1.06L12 21.23l7.78-7.78 1.06-1.06a5.5 5.5 0 000-7.78z"
                />
              </svg>
            </button>
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
