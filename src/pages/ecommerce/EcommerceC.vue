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
        <div class="mb-6 w-full lg:mb-0 lg:w-1/2 lg:py-6 lg:pr-10">
          <h2 class="title-font text-sm tracking-widest text-gray-500">
            BRAND NAME
          </h2>
          <h1 class="title-font mb-4 text-3xl font-medium text-gray-900 dark:text-white">
            Animated Night Hill Illustrations
          </h1>
          <div class="mb-4 flex">
            <a
              :class="`flex-grow text-${theme}-500 border-b-2 border-${theme}-500 py-2 text-lg px-1 dark:text-${theme}-400`"
            >Description</a>
            <a class="flex-grow border-b-2 border-gray-300 px-1 py-2 text-lg dark:border-gray-800">Reviews</a>
            <a class="flex-grow border-b-2 border-gray-300 px-1 py-2 text-lg dark:border-gray-800">Details</a>
          </div>
          <p class="mb-4 leading-relaxed">
            Fam locavore kickstarter distillery. Mixtape chillwave tumeric sriracha taximy chia microdosing tilde DIY.
            XOXO fam inxigo juiceramps cornhole raw denim forage brooklyn. Everyday carry +1 seitan poutine tumeric.
            Gastropub blue bottle austin listicle pour-over, neutra jean.
          </p>
          <div class="flex border-t border-gray-200 py-2 dark:border-gray-800">
            <span class="text-gray-500">Color</span>
            <span class="ml-auto text-gray-900 dark:text-white">Blue</span>
          </div>
          <div class="flex border-t border-gray-200 py-2 dark:border-gray-800">
            <span class="text-gray-500">Size</span>
            <span class="ml-auto text-gray-900 dark:text-white">Medium</span>
          </div>
          <div class="mb-6 flex border-b border-t border-gray-200 py-2 dark:border-gray-800">
            <span class="text-gray-500">Quantity</span>
            <span class="ml-auto text-gray-900 dark:text-white">4</span>
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
        <img
          alt="ecommerce" class="h-64 w-full rounded object-cover object-center lg:h-auto lg:w-1/2"
          src="https://dummyimage.com/400x400"
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
