<!--
  This example requires some changes to your config:

  ```
  // tailwind.config.js
  module.exports = {
    // ...
    plugins: [
      // ...
      require('@tailwindcss/aspect-ratio'),
    ],
  }
  ```
-->
<template>
  <div class="bg-gray-50">
    <div class="mx-auto max-w-7xl px-4 py-16 lg:px-8 sm:px-6 sm:py-24">
      <div class="sm:flex sm:items-baseline sm:justify-between">
        <h2 class="text-2xl font-bold tracking-tight text-gray-900">
          Shop by Category
        </h2>
        <a href="#" class="hidden text-sm font-semibold text-indigo-600 sm:block hover:text-indigo-500">
          Browse all categories
          <span aria-hidden="true"> &rarr;</span>
        </a>
      </div>

      <div class="grid grid-cols-1 mt-6 gap-y-6 sm:grid-cols-2 sm:grid-rows-2 lg:gap-8 sm:gap-x-6">
        <div class="group aspect-h-1 sm:aspect-h-1 aspect-w-2 sm:aspect-w-1 overflow-hidden rounded-lg sm:row-span-2">
          <img src="https://tailwindui.com/img/ecommerce-images/home-page-03-featured-category.jpg" alt="Two models wearing women's black cotton crewneck tee and off-white cotton crewneck tee." class="object-cover object-center group-hover:opacity-75">
          <div aria-hidden="true" class="from-transparent to-black bg-gradient-to-b opacity-50" />
          <div class="flex items-end p-6">
            <div>
              <h3 class="font-semibold text-white">
                <a href="#">
                  <span class="absolute inset-0" />
                  New Arrivals
                </a>
              </h3>
              <p aria-hidden="true" class="mt-1 text-sm text-white">
                Shop now
              </p>
            </div>
          </div>
        </div>
        <div class="group aspect-w-2 aspect-h-1 sm:aspect-none overflow-hidden rounded-lg sm:relative sm:h-full">
          <img src="https://tailwindui.com/img/ecommerce-images/home-page-03-category-01.jpg" alt="Wooden shelf with gray and olive drab green baseball caps, next to wooden clothes hanger with sweaters." class="object-cover object-center sm:absolute sm:inset-0 sm:h-full sm:w-full group-hover:opacity-75">
          <div aria-hidden="true" class="from-transparent to-black bg-gradient-to-b opacity-50 sm:absolute sm:inset-0" />
          <div class="flex items-end p-6 sm:absolute sm:inset-0">
            <div>
              <h3 class="font-semibold text-white">
                <a href="#">
                  <span class="absolute inset-0" />
                  Accessories
                </a>
              </h3>
              <p aria-hidden="true" class="mt-1 text-sm text-white">
                Shop now
              </p>
            </div>
          </div>
        </div>
        <div class="group aspect-w-2 aspect-h-1 sm:aspect-none overflow-hidden rounded-lg sm:relative sm:h-full">
          <img src="https://tailwindui.com/img/ecommerce-images/home-page-03-category-02.jpg" alt="Walnut desk organizer set with white modular trays, next to porcelain mug on wooden desk." class="object-cover object-center sm:absolute sm:inset-0 sm:h-full sm:w-full group-hover:opacity-75">
          <div aria-hidden="true" class="from-transparent to-black bg-gradient-to-b opacity-50 sm:absolute sm:inset-0" />
          <div class="flex items-end p-6 sm:absolute sm:inset-0">
            <div>
              <h3 class="font-semibold text-white">
                <a href="#">
                  <span class="absolute inset-0" />
                  Workspace
                </a>
              </h3>
              <p aria-hidden="true" class="mt-1 text-sm text-white">
                Shop now
              </p>
            </div>
          </div>
        </div>
      </div>

      <div class="mt-6 sm:hidden">
        <a href="#" class="block text-sm font-semibold text-indigo-600 hover:text-indigo-500">
          Browse all categories
          <span aria-hidden="true"> &rarr;</span>
        </a>
      </div>
    </div>
  </div>
</template>
