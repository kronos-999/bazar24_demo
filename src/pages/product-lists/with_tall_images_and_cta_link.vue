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
    name: 'Black Basic Tee',
    price: '$32',
    href: '#',
    imageSrc: 'https://tailwindui.com/img/ecommerce-images/home-page-03-favorite-01.jpg',
    imageAlt: 'Model wearing women\'s black cotton crewneck tee.',
  },
  // More products...
]
</script>

<template>
  <div class="bg-white">
    <div class="mx-auto max-w-7xl px-4 py-16 lg:px-8 sm:px-6 sm:py-24">
      <div class="sm:flex sm:items-baseline sm:justify-between">
        <h2 class="text-2xl font-bold tracking-tight text-gray-900">
          Our Favorites
        </h2>
        <a href="#" class="hidden text-sm font-semibold text-indigo-600 sm:block hover:text-indigo-500">
          Browse all favorites
          <span aria-hidden="true"> &rarr;</span>
        </a>
      </div>

      <div class="grid grid-cols-1 mt-6 gap-y-10 sm:grid-cols-3 lg:gap-x-8 sm:gap-x-6 sm:gap-y-0">
        <div v-for="product in products" :key="product.id" class="group relative">
          <div
            class="sm:aspect-w-2 sm:aspect-h-3 h-96 w-full overflow-hidden rounded-lg sm:h-auto group-hover:opacity-75"
          >
            <img :src="product.imageSrc" :alt="product.imageAlt" class="h-full w-full object-cover object-center">
          </div>
          <h3 class="mt-4 text-base font-semibold text-gray-900">
            <a :href="product.href">
              <span class="absolute inset-0" />
              {{ product.name }}
            </a>
          </h3>
          <p class="mt-1 text-sm text-gray-500">
            {{ product.price }}
          </p>
        </div>
      </div>

      <div class="mt-6 sm:hidden">
        <a href="#" class="block text-sm font-semibold text-indigo-600 hover:text-indigo-500">
          Browse all favorites
          <span aria-hidden="true"> &rarr;</span>
        </a>
      </div>
    </div>
  </div>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>
