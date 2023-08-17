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
    name: 'Basic Tee',
    href: '#',
    imageSrc: 'https://tailwindui.com/img/ecommerce-images/product-page-01-related-product-01.jpg',
    imageAlt: 'Front of men\'s Basic Tee in black.',
    price: '$35',
    color: 'Black',
  },
  // More products...
]
</script>

<template>
  <div class="bg-white">
    <div class="mx-auto max-w-2xl px-4 py-16 lg:max-w-7xl lg:px-8 sm:px-6 sm:py-24">
      <h2 class="text-2xl font-bold tracking-tight text-gray-900">
        Customers also purchased
      </h2>

      <div class="grid grid-cols-1 mt-6 gap-x-6 gap-y-10 lg:grid-cols-4 sm:grid-cols-2 xl:gap-x-8">
        <div v-for="product in products" :key="product.id" class="group relative">
          <div
            class="aspect-w-1 aspect-h-1 lg:aspect-none min-h-80 w-full overflow-hidden rounded-md bg-gray-200 lg:h-80 group-hover:opacity-75"
          >
            <img
              :src="product.imageSrc" :alt="product.imageAlt"
              class="h-full w-full object-cover object-center lg:h-full lg:w-full"
            >
          </div>
          <div class="mt-4 flex justify-between">
            <div>
              <h3 class="text-sm text-gray-700">
                <a :href="product.href">
                  <span aria-hidden="true" class="absolute inset-0" />
                  {{ product.name }}
                </a>
              </h3>
              <p class="mt-1 text-sm text-gray-500">
                {{ product.color }}
              </p>
            </div>
            <p class="text-sm font-medium text-gray-900">
              {{ product.price }}
            </p>
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
