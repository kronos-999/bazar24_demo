<script setup>
const categories = [
  {
    name: 'New Arrivals',
    href: '#',
    imageSrc: 'https://tailwindui.com/img/ecommerce-images/home-page-01-category-01.jpg',
  },
  {
    name: 'Productivity',
    href: '#',
    imageSrc: 'https://tailwindui.com/img/ecommerce-images/home-page-01-category-02.jpg',
  },
  {
    name: 'Workspace',
    href: '#',
    imageSrc: 'https://tailwindui.com/img/ecommerce-images/home-page-01-category-04.jpg',
  },
  {
    name: 'Accessories',
    href: '#',
    imageSrc: 'https://tailwindui.com/img/ecommerce-images/home-page-01-category-05.jpg',
  },
  { name: 'Sale', href: '#', imageSrc: 'https://tailwindui.com/img/ecommerce-images/home-page-01-category-03.jpg' },
]
</script>

<template>
  <div class="bg-white">
    <div class="py-16 xl:mx-auto xl:max-w-7xl sm:py-24 xl:px-8">
      <div class="px-4 sm:flex sm:items-center sm:justify-between lg:px-8 sm:px-6 xl:px-0">
        <h2 class="text-2xl font-bold tracking-tight text-gray-900">
          Shop by Category
        </h2>
        <a href="#" class="hidden text-sm font-semibold text-indigo-600 sm:block hover:text-indigo-500">
          Browse all categories
          <span aria-hidden="true"> &rarr;</span>
        </a>
      </div>

      <div class="mt-4 flow-root">
        <div class="-my-2">
          <div class="relative box-content h-80 overflow-x-auto py-2 xl:overflow-visible">
            <div
              class="absolute min-w-screen-xl flex px-4 xl:relative xl:grid xl:grid-cols-5 xl:gap-x-8 space-x-8 lg:px-8 sm:px-6 xl:px-0 xl:space-x-0"
            >
              <a
                v-for="category in categories" :key="category.name" :href="category.href"
                class="relative h-80 w-56 flex flex-col overflow-hidden rounded-lg p-6 xl:w-auto hover:opacity-75"
              >
                <span aria-hidden="true" class="absolute inset-0">
                  <img :src="category.imageSrc" alt="" class="h-full w-full object-cover object-center">
                </span>
                <span
                  aria-hidden="true"
                  class="absolute inset-x-0 bottom-0 h-2/3 from-gray-800 bg-gradient-to-t opacity-50"
                />
                <span class="relative mt-auto text-center text-xl font-bold text-white">{{ category.name }}</span>
              </a>
            </div>
          </div>
        </div>
      </div>

      <div class="mt-6 px-4 sm:hidden">
        <a href="#" class="block text-sm font-semibold text-indigo-600 hover:text-indigo-500">
          Browse all categories
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
