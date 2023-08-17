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
<script setup>
const products = [
  {
    id: 1,
    name: 'Basic Tee 8-Pack',
    href: '#',
    price: '$256',
    description: 'Get the full lineup of our Basic Tees. Have a fresh shirt all week, and an extra for laundry day.',
    options: '8 colors',
    imageSrc: 'https://tailwindui.com/img/ecommerce-images/category-page-02-image-card-01.jpg',
    imageAlt: 'Eight shirts arranged on table in black, olive, grey, blue, white, red, mustard, and green.',
  },
  {
    id: 2,
    name: 'Basic Tee',
    href: '#',
    price: '$32',
    description: 'Look like a visionary CEO and wear the same black t-shirt every day.',
    options: 'Black',
    imageSrc: 'https://tailwindui.com/img/ecommerce-images/category-page-02-image-card-02.jpg',
    imageAlt: 'Front of plain black t-shirt.',
  },
  // More products...
]
</script>

<template>
  <div class="bg-white">
    <div class="mx-auto max-w-2xl px-4 py-16 lg:max-w-7xl lg:px-8 sm:px-6 sm:py-24">
      <h2 class="sr-only">
        Products
      </h2>

      <div class="grid grid-cols-1 gap-y-4 lg:grid-cols-3 sm:grid-cols-2 lg:gap-x-8 sm:gap-x-6 sm:gap-y-10">
        <div
          v-for="product in products" :key="product.id"
          class="group relative flex flex-col overflow-hidden border border-gray-200 rounded-lg bg-white"
        >
          <div class="aspect-w-3 aspect-h-4 sm:aspect-none bg-gray-200 sm:h-96 group-hover:opacity-75">
            <img
              :src="product.imageSrc" :alt="product.imageAlt"
              class="h-full w-full object-cover object-center sm:h-full sm:w-full"
            >
          </div>
          <div class="flex flex-1 flex-col p-4 space-y-2">
            <h3 class="text-sm font-medium text-gray-900">
              <a :href="product.href">
                <span aria-hidden="true" class="absolute inset-0" />
                {{ product.name }}
              </a>
            </h3>
            <p class="text-sm text-gray-500">
              {{ product.description }}
            </p>
            <div class="flex flex-1 flex-col justify-end">
              <p class="text-sm italic text-gray-500">
                {{ product.options }}
              </p>
              <p class="text-base font-medium text-gray-900">
                {{ product.price }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>
