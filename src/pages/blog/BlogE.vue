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
      <div class="flex flex-wrap -mx-4 -my-8">
        <div class="px-4 py-8 lg:w-1/3">
          <div class="h-full flex items-start">
            <div class="w-12 flex flex-shrink-0 flex-col text-center leading-none">
              <span
                class="mb-2 border-b-2 border-gray-200 pb-2 text-gray-500 dark:border-gray-700 dark:text-gray-400"
              >Jul</span>
              <span class="title-font text-lg font-medium leading-none text-gray-800 dark:text-gray-300">18</span>
            </div>
            <div class="flex-grow pl-6">
              <h2 :class="`tracking-widest text-xs title-font font-medium text-${theme}-500 mb-1 dark:text-${theme}-400`">
                CATEGORY
              </h2>
              <h1 class="title-font mb-3 text-xl font-medium text-gray-900 dark:text-white">
                The 400 Blows
              </h1>
              <p class="mb-5 leading-relaxed">
                Photo booth fam kinfolk cold-pressed sriracha leggings jianbing microdosing tousled waistcoat.
              </p>
              <a class="inline-flex items-center">
                <img
                  alt="blog" src="https://dummyimage.com/103x103"
                  class="h-8 w-8 flex-shrink-0 rounded-full object-cover object-center"
                >
                <span class="flex flex-grow flex-col pl-3">
                  <span class="title-font font-medium text-gray-900 dark:text-white">Alper Kamu</span>
                </span>
              </a>
            </div>
          </div>
        </div>
        <div class="px-4 py-8 lg:w-1/3">
          <div class="h-full flex items-start">
            <div class="w-12 flex flex-shrink-0 flex-col text-center leading-none">
              <span
                class="mb-2 border-b-2 border-gray-200 pb-2 text-gray-500 dark:border-gray-700 dark:text-gray-400"
              >Jul</span>
              <span class="title-font text-lg font-medium leading-none text-gray-800 dark:text-gray-300">18</span>
            </div>
            <div class="flex-grow pl-6">
              <h2 :class="`tracking-widest text-xs title-font font-medium text-${theme}-500 mb-1 dark:text-${theme}-400`">
                CATEGORY
              </h2>
              <h1 class="title-font mb-3 text-xl font-medium text-gray-900 dark:text-white">
                Shooting Stars
              </h1>
              <p class="mb-5 leading-relaxed">
                Photo booth fam kinfolk cold-pressed sriracha leggings jianbing microdosing tousled waistcoat.
              </p>
              <a class="inline-flex items-center">
                <img
                  alt="blog" src="https://dummyimage.com/102x102"
                  class="h-8 w-8 flex-shrink-0 rounded-full object-cover object-center"
                >
                <span class="flex flex-grow flex-col pl-3">
                  <span class="title-font font-medium text-gray-900 dark:text-white">Holden Caulfield</span>
                </span>
              </a>
            </div>
          </div>
        </div>
        <div class="px-4 py-8 lg:w-1/3">
          <div class="h-full flex items-start">
            <div class="w-12 flex flex-shrink-0 flex-col text-center leading-none">
              <span
                class="mb-2 border-b-2 border-gray-200 pb-2 text-gray-500 dark:border-gray-700 dark:text-gray-400"
              >Jul</span>
              <span class="title-font text-lg font-medium leading-none text-gray-800 dark:text-gray-300">18</span>
            </div>
            <div class="flex-grow pl-6">
              <h2 :class="`tracking-widest text-xs title-font font-medium text-${theme}-500 mb-1 dark:text-${theme}-400`">
                CATEGORY
              </h2>
              <h1 class="title-font mb-3 text-xl font-medium text-gray-900 dark:text-white">
                Neptune
              </h1>
              <p class="mb-5 leading-relaxed">
                Photo booth fam kinfolk cold-pressed sriracha leggings jianbing microdosing tousled waistcoat.
              </p>
              <a class="inline-flex items-center">
                <img
                  alt="blog" src="https://dummyimage.com/101x101"
                  class="h-8 w-8 flex-shrink-0 rounded-full object-cover object-center"
                >
                <span class="flex flex-grow flex-col pl-3">
                  <span class="title-font font-medium text-gray-900 dark:text-white">Henry Letham</span>
                </span>
              </a>
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
