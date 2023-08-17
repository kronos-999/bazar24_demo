<!--
  This example requires some changes to your config:

  ```
  // tailwind.config.js
  module.exports = {
    // ...
    plugins: [
      // ...
      require('@tailwindcss/forms'),
      require('@tailwindcss/aspect-ratio'),
    ],
  }
  ```
-->
<script setup>
import { ref } from 'vue'
import {
  Dialog,
  DialogPanel,
  Popover,
  PopoverButton,
  PopoverGroup,
  PopoverPanel,
  Tab,
  TabGroup,
  TabList,
  TabPanel,
  TabPanels,
  TransitionChild,
  TransitionRoot,
} from '@headlessui/vue'
import { Bars3Icon, MagnifyingGlassIcon, ShoppingBagIcon, UserIcon, XMarkIcon } from '@heroicons/vue/24/outline'
import { CheckIcon, ClockIcon } from '@heroicons/vue/20/solid'

const navigation = {
  categories: [
    {
      id: 'women',
      name: 'Women',
      featured: [
        {
          name: 'New Arrivals',
          href: '#',
          imageSrc: 'https://tailwindui.com/img/ecommerce-images/mega-menu-category-01.jpg',
          imageAlt: 'Models sitting back to back, wearing Basic Tee in black and bone.',
        },
        {
          name: 'Basic Tees',
          href: '#',
          imageSrc: 'https://tailwindui.com/img/ecommerce-images/mega-menu-category-02.jpg',
          imageAlt: 'Close up of Basic Tee fall bundle with off-white, ochre, olive, and black tees.',
        },
        {
          name: 'Accessories',
          href: '#',
          imageSrc: 'https://tailwindui.com/img/ecommerce-images/mega-menu-category-03.jpg',
          imageAlt: 'Model wearing minimalist watch with black wristband and white watch face.',
        },
      ],
      sections: [
        [
          {
            id: 'shoes',
            name: 'Shoes & Accessories',
            items: [
              { name: 'Sneakers', href: '#' },
              { name: 'Boots', href: '#' },
              { name: 'Flats', href: '#' },
              { name: 'Sandals', href: '#' },
              { name: 'Heels', href: '#' },
              { name: 'Socks', href: '#' },
            ],
          },
          {
            id: 'collection',
            name: 'Shop Collection',
            items: [
              { name: 'Everything', href: '#' },
              { name: 'Core', href: '#' },
              { name: 'New Arrivals', href: '#' },
              { name: 'Sale', href: '#' },
              { name: 'Accessories', href: '#' },
            ],
          },
        ],
        [
          {
            id: 'clothing',
            name: 'All Clothing',
            items: [
              { name: 'Basic Tees', href: '#' },
              { name: 'Artwork Tees', href: '#' },
              { name: 'Tops', href: '#' },
              { name: 'Bottoms', href: '#' },
              { name: 'Swimwear', href: '#' },
              { name: 'Underwear', href: '#' },
            ],
          },
          {
            id: 'accessories',
            name: 'All Accessories',
            items: [
              { name: 'Watches', href: '#' },
              { name: 'Wallets', href: '#' },
              { name: 'Bags', href: '#' },
              { name: 'Sunglasses', href: '#' },
              { name: 'Hats', href: '#' },
              { name: 'Belts', href: '#' },
            ],
          },
        ],
        [
          {
            id: 'brands',
            name: 'Brands',
            items: [
              { name: 'Full Nelson', href: '#' },
              { name: 'My Way', href: '#' },
              { name: 'Re-Arranged', href: '#' },
              { name: 'Counterfeit', href: '#' },
              { name: 'Significant Other', href: '#' },
            ],
          },
        ],
      ],
    },
    {
      id: 'men',
      name: 'Men',
      featured: [
        {
          name: 'Accessories',
          href: '#',
          imageSrc: 'https://tailwindui.com/img/ecommerce-images/home-page-03-category-01.jpg',
          imageAlt:
            'Wooden shelf with gray and olive drab green baseball caps, next to wooden clothes hanger with sweaters.',
        },
        {
          name: 'New Arrivals',
          href: '#',
          imageSrc: 'https://tailwindui.com/img/ecommerce-images/product-page-04-detail-product-shot-01.jpg',
          imageAlt: 'Drawstring top with elastic loop closure and textured interior padding.',
        },
        {
          name: 'Artwork Tees',
          href: '#',
          imageSrc: 'https://tailwindui.com/img/ecommerce-images/category-page-02-image-card-06.jpg',
          imageAlt:
            'Three shirts in gray, white, and blue arranged on table with same line drawing of hands and shapes overlapping on front of shirt.',
        },
      ],
      sections: [
        [
          {
            id: 'shoes',
            name: 'Shoes & Accessories',
            items: [
              { name: 'Sneakers', href: '#' },
              { name: 'Boots', href: '#' },
              { name: 'Sandals', href: '#' },
              { name: 'Socks', href: '#' },
            ],
          },
          {
            id: 'collection',
            name: 'Shop Collection',
            items: [
              { name: 'Everything', href: '#' },
              { name: 'Core', href: '#' },
              { name: 'New Arrivals', href: '#' },
              { name: 'Sale', href: '#' },
            ],
          },
        ],
        [
          {
            id: 'clothing',
            name: 'All Clothing',
            items: [
              { name: 'Basic Tees', href: '#' },
              { name: 'Artwork Tees', href: '#' },
              { name: 'Pants', href: '#' },
              { name: 'Hoodies', href: '#' },
              { name: 'Swimsuits', href: '#' },
            ],
          },
          {
            id: 'accessories',
            name: 'All Accessories',
            items: [
              { name: 'Watches', href: '#' },
              { name: 'Wallets', href: '#' },
              { name: 'Bags', href: '#' },
              { name: 'Sunglasses', href: '#' },
              { name: 'Hats', href: '#' },
              { name: 'Belts', href: '#' },
            ],
          },
        ],
        [
          {
            id: 'brands',
            name: 'Brands',
            items: [
              { name: 'Re-Arranged', href: '#' },
              { name: 'Counterfeit', href: '#' },
              { name: 'Full Nelson', href: '#' },
              { name: 'My Way', href: '#' },
            ],
          },
        ],
      ],
    },
  ],
  pages: [
    { name: 'Company', href: '#' },
    { name: 'Stores', href: '#' },
  ],
}
const products = [
  {
    id: 1,
    name: 'Nomad Tumbler',
    href: '#',
    price: '$35.00',
    color: 'White',
    inStock: true,
    imageSrc: 'https://tailwindui.com/img/ecommerce-images/shopping-cart-page-01-product-03.jpg',
    imageAlt: 'Insulated bottle with white base and black snap lid.',
  },
  {
    id: 2,
    name: 'Basic Tee',
    href: '#',
    price: '$32.00',
    color: 'Sienna',
    inStock: true,
    size: 'Large',
    imageSrc: 'https://tailwindui.com/img/ecommerce-images/shopping-cart-page-01-product-01.jpg',
    imageAlt: 'Front of men\'s Basic Tee in sienna.',
  },
  // More products...
]
const policies = [
  {
    name: 'Free returns',
    imageSrc: 'https://tailwindui.com/img/ecommerce/icons/icon-returns-light.svg',
    description: 'Not what you expected? Place it back in the parcel and attach the pre-paid postage stamp.',
  },
  {
    name: 'Same day delivery',
    imageSrc: 'https://tailwindui.com/img/ecommerce/icons/icon-calendar-light.svg',
    description:
      'We offer a delivery service that has never been done before. Checkout today and receive your products within hours.',
  },
  {
    name: 'All year discount',
    imageSrc: 'https://tailwindui.com/img/ecommerce/icons/icon-gift-card-light.svg',
    description: 'Looking for a deal? You can use the code "ALLYEAR" at checkout and get money off all year round.',
  },
  {
    name: 'For the planet',
    imageSrc: 'https://tailwindui.com/img/ecommerce/icons/icon-planet-light.svg',
    description: 'We’ve pledged 1% of sales to the preservation and restoration of the natural environment.',
  },
]
const footerNavigation = {
  products: [
    { name: 'Bags', href: '#' },
    { name: 'Tees', href: '#' },
    { name: 'Objects', href: '#' },
    { name: 'Home Goods', href: '#' },
    { name: 'Accessories', href: '#' },
  ],
  company: [
    { name: 'Who we are', href: '#' },
    { name: 'Sustainability', href: '#' },
    { name: 'Press', href: '#' },
    { name: 'Careers', href: '#' },
    { name: 'Terms & Conditions', href: '#' },
    { name: 'Privacy', href: '#' },
  ],
  customerService: [
    { name: 'Contact', href: '#' },
    { name: 'Shipping', href: '#' },
    { name: 'Returns', href: '#' },
    { name: 'Warranty', href: '#' },
    { name: 'Secure Payments', href: '#' },
    { name: 'FAQ', href: '#' },
    { name: 'Find a store', href: '#' },
  ],
}

const open = ref(false)
</script>

<template>
  <div class="bg-white">
    <!-- Mobile menu -->
    <TransitionRoot as="template" :show="open">
      <Dialog as="div" class="relative z-40 lg:hidden" @close="open = false">
        <TransitionChild
          as="template" enter="transition-opacity ease-linear duration-300" enter-from="opacity-0"
          enter-to="opacity-100" leave="transition-opacity ease-linear duration-300" leave-from="opacity-100"
          leave-to="opacity-0"
        >
          <div class="fixed inset-0 bg-black bg-opacity-25" />
        </TransitionChild>

        <div class="fixed inset-0 z-40 flex">
          <TransitionChild
            as="template" enter="transition ease-in-out duration-300 transform"
            enter-from="-translate-x-full" enter-to="translate-x-0" leave="transition ease-in-out duration-300 transform"
            leave-from="translate-x-0" leave-to="-translate-x-full"
          >
            <DialogPanel class="relative max-w-xs w-full flex flex-col overflow-y-auto bg-white pb-12 shadow-xl">
              <div class="flex px-4 pb-2 pt-5">
                <button
                  type="button" class="inline-flex items-center justify-center rounded-md p-2 text-gray-400 -m-2"
                  @click="open = false"
                >
                  <span class="sr-only">Close menu</span>
                  <XMarkIcon class="h-6 w-6" aria-hidden="true" />
                </button>
              </div>

              <!-- Links -->
              <TabGroup as="div" class="mt-2">
                <div class="border-b border-gray-200">
                  <TabList class="flex px-4 -mb-px space-x-8">
                    <Tab
                      v-for="category in navigation.categories" :key="category.name" v-slot="{ selected }"
                      as="template"
                    >
                      <button
                        class="flex-1 whitespace-nowrap border-b-2 px-1 py-4 text-base font-medium" :class="[selected ? 'text-indigo-600 border-indigo-600' : 'text-gray-900 border-transparent']"
                      >
                        {{ category.name }}
                      </button>
                    </Tab>
                  </TabList>
                </div>
                <TabPanels as="template">
                  <TabPanel
                    v-for="category in navigation.categories" :key="category.name"
                    class="px-4 pb-8 pt-10 space-y-10"
                  >
                    <div class="space-y-4">
                      <div
                        v-for="(item, itemIdx) in category.featured" :key="itemIdx"
                        class="group aspect-w-1 aspect-h-1 relative overflow-hidden rounded-md bg-gray-100"
                      >
                        <img
                          :src="item.imageSrc" :alt="item.imageAlt"
                          class="object-cover object-center group-hover:opacity-75"
                        >
                        <div class="flex flex-col justify-end">
                          <div class="bg-white bg-opacity-60 p-4 text-base sm:text-sm">
                            <a :href="item.href" class="font-medium text-gray-900">
                              <span class="absolute inset-0" aria-hidden="true" />
                              {{ item.name }}
                            </a>
                            <p aria-hidden="true" class="mt-0.5 text-gray-700 sm:mt-1">
                              Shop now
                            </p>
                          </div>
                        </div>
                      </div>
                    </div>
                    <div v-for="(column, columnIdx) in category.sections" :key="columnIdx" class="space-y-10">
                      <div v-for="section in column" :key="section.name">
                        <p :id="`${category.id}-${section.id}-heading-mobile`" class="font-medium text-gray-900">
                          {{ section.name }}
                        </p>
                        <ul
                          role="list" :aria-labelledby="`${category.id}-${section.id}-heading-mobile`"
                          class="mt-6 flex flex-col space-y-6"
                        >
                          <li v-for="item in section.items" :key="item.name" class="flow-root">
                            <a :href="item.href" class="block p-2 text-gray-500 -m-2">{{ item.name }}</a>
                          </li>
                        </ul>
                      </div>
                    </div>
                  </TabPanel>
                </TabPanels>
              </TabGroup>

              <div class="border-t border-gray-200 px-4 py-6 space-y-6">
                <div v-for="page in navigation.pages" :key="page.name" class="flow-root">
                  <a :href="page.href" class="block p-2 font-medium text-gray-900 -m-2">{{ page.name }}</a>
                </div>
              </div>

              <div class="border-t border-gray-200 px-4 py-6">
                <a href="#" class="flex items-center p-2 -m-2">
                  <img
                    src="https://tailwindui.com/img/flags/flag-canada.svg" alt=""
                    class="block h-auto w-5 flex-shrink-0"
                  >
                  <span class="ml-3 block text-base font-medium text-gray-900">CAD</span>
                  <span class="sr-only">, change currency</span>
                </a>
              </div>
            </DialogPanel>
          </TransitionChild>
        </div>
      </Dialog>
    </TransitionRoot>

    <header class="relative bg-white">
      <nav aria-label="Top" class="mx-auto max-w-7xl px-4 lg:px-8 sm:px-6">
        <div class="border-b border-gray-200">
          <div class="h-16 flex items-center justify-between">
            <div class="flex flex-1 items-center lg:hidden">
              <button type="button" class="rounded-md bg-white p-2 text-gray-400 -ml-2" @click="open = true">
                <span class="sr-only">Open menu</span>
                <Bars3Icon class="h-6 w-6" aria-hidden="true" />
              </button>

              <a href="#" class="ml-2 p-2 text-gray-400 hover:text-gray-500">
                <span class="sr-only">Search</span>
                <MagnifyingGlassIcon class="h-6 w-6" aria-hidden="true" />
              </a>
            </div>

            <!-- Flyout menus -->
            <PopoverGroup class="hidden lg:block lg:flex-1 lg:self-stretch">
              <div class="h-full flex space-x-8">
                <Popover v-for="category in navigation.categories" :key="category.name" v-slot="{ open }" class="flex">
                  <div class="relative flex">
                    <PopoverButton
                      class="relative z-10 flex items-center justify-center text-sm font-medium transition-colors duration-200 ease-out" :class="[open ? 'text-indigo-600' : 'text-gray-700 hover:text-gray-800']"
                    >
                      {{ category.name }}
                      <span
                        class="absolute inset-x-0 bottom-0 h-0.5 transition-colors duration-200 ease-out sm:mt-5 sm:translate-y-px sm:transform" :class="[open ? 'bg-indigo-600' : '']"
                        aria-hidden="true"
                      />
                    </PopoverButton>
                  </div>

                  <transition
                    enter-active-class="transition ease-out duration-200" enter-from-class="opacity-0"
                    enter-to-class="opacity-100" leave-active-class="transition ease-in duration-150"
                    leave-from-class="opacity-100" leave-to-class="opacity-0"
                  >
                    <PopoverPanel class="absolute inset-x-0 top-full z-10">
                      <!-- Presentational element used to render the bottom shadow, if we put the shadow on the actual panel it pokes out the top, so we use this shorter element to hide the top of the shadow -->
                      <div class="absolute inset-0 top-1/2 bg-white shadow" aria-hidden="true" />

                      <div class="relative bg-white">
                        <div class="mx-auto max-w-7xl px-8">
                          <div class="grid grid-cols-2 gap-x-8 gap-y-10 py-16">
                            <div class="grid grid-cols-2 grid-rows-1 gap-8 text-sm">
                              <div
                                v-for="(item, itemIdx) in category.featured" :key="item.name"
                                class="group aspect-w-1 aspect-h-1 relative overflow-hidden rounded-md bg-gray-100" :class="[itemIdx === 0 ? 'col-span-2 aspect-w-2' : '']"
                              >
                                <img
                                  :src="item.imageSrc" :alt="item.imageAlt"
                                  class="object-cover object-center group-hover:opacity-75"
                                >
                                <div class="flex flex-col justify-end">
                                  <div class="bg-white bg-opacity-60 p-4 text-sm">
                                    <a :href="item.href" class="font-medium text-gray-900">
                                      <span class="absolute inset-0" aria-hidden="true" />
                                      {{ item.name }}
                                    </a>
                                    <p aria-hidden="true" class="mt-0.5 text-gray-700 sm:mt-1">
                                      Shop now
                                    </p>
                                  </div>
                                </div>
                              </div>
                            </div>
                            <div class="grid grid-cols-3 gap-x-8 gap-y-10 text-sm text-gray-500">
                              <div v-for="(column, columnIdx) in category.sections" :key="columnIdx" class="space-y-10">
                                <div v-for="section in column" :key="section.name">
                                  <p :id="`${category.id}-${section.id}-heading`" class="font-medium text-gray-900">
                                    {{ section.name }}
                                  </p>
                                  <ul
                                    role="list" :aria-labelledby="`${category.id}-${section.id}-heading`"
                                    class="mt-4 space-y-4"
                                  >
                                    <li v-for="item in section.items" :key="item.name" class="flex">
                                      <a :href="item.href" class="hover:text-gray-800">{{ item.name }}</a>
                                    </li>
                                  </ul>
                                </div>
                              </div>
                            </div>
                          </div>
                        </div>
                      </div>
                    </PopoverPanel>
                  </transition>
                </Popover>

                <a
                  v-for="page in navigation.pages" :key="page.name" :href="page.href"
                  class="flex items-center text-sm font-medium text-gray-700 hover:text-gray-800"
                >{{ page.name }}</a>
              </div>
            </PopoverGroup>

            <!-- Logo -->
            <a href="#" class="flex">
              <span class="sr-only">Your Company</span>
              <img class="h-8 w-auto" src="https://tailwindui.com/img/logos/mark.svg?color=indigo&shade=600" alt="">
            </a>

            <div class="flex flex-1 items-center justify-end">
              <a href="#" class="hidden text-gray-700 lg:flex lg:items-center hover:text-gray-800">
                <img
                  src="https://tailwindui.com/img/flags/flag-canada.svg" alt=""
                  class="block h-auto w-5 flex-shrink-0"
                >
                <span class="ml-3 block text-sm font-medium">CAD</span>
                <span class="sr-only">, change currency</span>
              </a>

              <!-- Search -->
              <a href="#" class="ml-6 hidden p-2 text-gray-400 lg:block hover:text-gray-500">
                <span class="sr-only">Search</span>
                <MagnifyingGlassIcon class="h-6 w-6" aria-hidden="true" />
              </a>

              <!-- Account -->
              <a href="#" class="p-2 text-gray-400 lg:ml-4 hover:text-gray-500">
                <span class="sr-only">Account</span>
                <UserIcon class="h-6 w-6" aria-hidden="true" />
              </a>

              <!-- Cart -->
              <div class="ml-4 flow-root lg:ml-6">
                <a href="#" class="group flex items-center p-2 -m-2">
                  <ShoppingBagIcon
                    class="h-6 w-6 flex-shrink-0 text-gray-400 group-hover:text-gray-500"
                    aria-hidden="true"
                  />
                  <span class="ml-2 text-sm font-medium text-gray-700 group-hover:text-gray-800">0</span>
                  <span class="sr-only">items in cart, view bag</span>
                </a>
              </div>
            </div>
          </div>
        </div>
      </nav>
    </header>

    <main>
      <div class="mx-auto max-w-7xl px-4 lg:px-8 sm:px-6">
        <div class="mx-auto max-w-4xl pt-16">
          <h1 class="text-3xl font-bold tracking-tight text-gray-900">
            Shopping Cart
          </h1>

          <form class="mt-12">
            <section aria-labelledby="cart-heading">
              <h2 id="cart-heading" class="sr-only">
                Items in your shopping cart
              </h2>

              <ul role="list" class="border-b border-t border-gray-200 divide-y divide-gray-200">
                <li v-for="(product, productIdx) in products" :key="product.id" class="flex py-6 sm:py-10">
                  <div class="flex-shrink-0">
                    <img
                      :src="product.imageSrc" :alt="product.imageAlt"
                      class="h-24 w-24 rounded-lg object-cover object-center sm:h-32 sm:w-32"
                    >
                  </div>

                  <div class="relative ml-4 flex flex-1 flex-col justify-between sm:ml-6">
                    <div>
                      <div class="flex justify-between sm:grid sm:grid-cols-2">
                        <div class="pr-6">
                          <h3 class="text-sm">
                            <a
                              :href="product.href"
                              class="font-medium text-gray-700 hover:text-gray-800"
                            >{{ product.name }}</a>
                          </h3>
                          <p class="mt-1 text-sm text-gray-500">
                            {{ product.color }}
                          </p>
                          <p v-if="product.size" class="mt-1 text-sm text-gray-500">
                            {{ product.size }}
                          </p>
                        </div>

                        <p class="text-right text-sm font-medium text-gray-900">
                          {{ product.price }}
                        </p>
                      </div>

                      <div class="mt-4 flex items-center sm:absolute sm:left-1/2 sm:top-0 sm:mt-0 sm:block">
                        <label :for="`quantity-${productIdx}`" class="sr-only">Quantity, {{ product.name }}</label>
                        <select
                          :id="`quantity-${productIdx}`" :name="`quantity-${productIdx}`"
                          class="block max-w-full border border-gray-300 rounded-md py-1.5 text-left text-base font-medium leading-5 text-gray-700 shadow-sm focus:border-indigo-500 sm:text-sm focus:outline-none focus:ring-1 focus:ring-indigo-500"
                        >
                          <option value="1">
                            1
                          </option>
                          <option value="2">
                            2
                          </option>
                          <option value="3">
                            3
                          </option>
                          <option value="4">
                            4
                          </option>
                          <option value="5">
                            5
                          </option>
                          <option value="6">
                            6
                          </option>
                          <option value="7">
                            7
                          </option>
                          <option value="8">
                            8
                          </option>
                        </select>

                        <button
                          type="button"
                          class="ml-4 text-sm font-medium text-indigo-600 sm:ml-0 sm:mt-3 hover:text-indigo-500"
                        >
                          <span>Remove</span>
                        </button>
                      </div>
                    </div>

                    <p class="mt-4 flex text-sm text-gray-700 space-x-2">
                      <CheckIcon v-if="product.inStock" class="h-5 w-5 flex-shrink-0 text-green-500" aria-hidden="true" />
                      <ClockIcon v-else class="h-5 w-5 flex-shrink-0 text-gray-300" aria-hidden="true" />
                      <span>{{ product.inStock ? 'In stock' : `Ships in ${product.leadTime}` }}</span>
                    </p>
                  </div>
                </li>
              </ul>
            </section>

            <!-- Order summary -->
            <section aria-labelledby="summary-heading" class="mt-10 sm:ml-32 sm:pl-6">
              <div class="rounded-lg bg-gray-50 px-4 py-6 lg:p-8 sm:p-6">
                <h2 id="summary-heading" class="sr-only">
                  Order summary
                </h2>

                <div class="flow-root">
                  <dl class="text-sm -my-4 divide-y divide-gray-200">
                    <div class="flex items-center justify-between py-4">
                      <dt class="text-gray-600">
                        Subtotal
                      </dt>
                      <dd class="font-medium text-gray-900">
                        $99.00
                      </dd>
                    </div>
                    <div class="flex items-center justify-between py-4">
                      <dt class="text-gray-600">
                        Shipping
                      </dt>
                      <dd class="font-medium text-gray-900">
                        $5.00
                      </dd>
                    </div>
                    <div class="flex items-center justify-between py-4">
                      <dt class="text-gray-600">
                        Tax
                      </dt>
                      <dd class="font-medium text-gray-900">
                        $8.32
                      </dd>
                    </div>
                    <div class="flex items-center justify-between py-4">
                      <dt class="text-base font-medium text-gray-900">
                        Order total
                      </dt>
                      <dd class="text-base font-medium text-gray-900">
                        $112.32
                      </dd>
                    </div>
                  </dl>
                </div>
              </div>
              <div class="mt-10">
                <button
                  type="submit"
                  class="w-full border border-transparent rounded-md bg-indigo-600 px-4 py-3 text-base font-medium text-white shadow-sm hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500 focus:ring-offset-gray-50"
                >
                  Checkout
                </button>
              </div>

              <div class="mt-6 text-center text-sm text-gray-500">
                <p>
                  or
                  <a href="#" class="font-medium text-indigo-600 hover:text-indigo-500">
                    Continue Shopping
                    <span aria-hidden="true"> &rarr;</span>
                  </a>
                </p>
              </div>
            </section>
          </form>
        </div>
      </div>

      <!-- Policy grid -->
      <section aria-labelledby="policies-heading" class="mt-24 border-t border-gray-200 bg-gray-50">
        <h2 id="policies-heading" class="sr-only">
          Our policies
        </h2>

        <div class="mx-auto max-w-7xl px-4 py-24 lg:px-8 sm:px-6 sm:py-32">
          <div class="grid grid-cols-1 gap-y-12 lg:grid-cols-4 sm:grid-cols-2 lg:gap-x-8 lg:gap-y-0 sm:gap-x-6">
            <div
              v-for="policy in policies" :key="policy.name"
              class="text-center lg:block md:flex md:items-start lg:text-center md:text-left"
            >
              <div class="md:flex-shrink-0">
                <div class="flow-root">
                  <img class="mx-auto h-24 w-auto -my-1" :src="policy.imageSrc" alt="">
                </div>
              </div>
              <div class="mt-6 lg:ml-0 lg:mt-6 md:ml-4 md:mt-0">
                <h3 class="text-base font-medium text-gray-900">
                  {{ policy.name }}
                </h3>
                <p class="mt-3 text-sm text-gray-500">
                  {{ policy.description }}
                </p>
              </div>
            </div>
          </div>
        </div>
      </section>
    </main>

    <footer aria-labelledby="footer-heading" class="bg-gray-50">
      <h2 id="footer-heading" class="sr-only">
        Footer
      </h2>
      <div class="mx-auto max-w-7xl px-4 lg:px-8 sm:px-6">
        <div class="border-t border-gray-200 py-20">
          <div class="grid grid-cols-1 md:auto-rows-min md:grid-flow-col md:grid-cols-12 md:gap-x-8 md:gap-y-16">
            <!-- Image section -->
            <div class="col-span-1 md:col-span-2 lg:col-start-1 lg:row-start-1">
              <img src="https://tailwindui.com/img/logos/mark.svg?color=indigo&shade=600" alt="" class="h-8 w-auto">
            </div>

            <!-- Sitemap sections -->
            <div
              class="grid col-span-6 grid-cols-2 mt-10 gap-8 lg:col-span-6 md:col-span-8 lg:col-start-2 md:col-start-3 md:row-start-1 sm:grid-cols-3 md:mt-0"
            >
              <div class="grid grid-cols-1 gap-y-12 sm:col-span-2 sm:grid-cols-2 sm:gap-x-8">
                <div>
                  <h3 class="text-sm font-medium text-gray-900">
                    Products
                  </h3>
                  <ul role="list" class="mt-6 space-y-6">
                    <li v-for="item in footerNavigation.products" :key="item.name" class="text-sm">
                      <a :href="item.href" class="text-gray-500 hover:text-gray-600">{{ item.name }}</a>
                    </li>
                  </ul>
                </div>
                <div>
                  <h3 class="text-sm font-medium text-gray-900">
                    Company
                  </h3>
                  <ul role="list" class="mt-6 space-y-6">
                    <li v-for="item in footerNavigation.company" :key="item.name" class="text-sm">
                      <a :href="item.href" class="text-gray-500 hover:text-gray-600">{{ item.name }}</a>
                    </li>
                  </ul>
                </div>
              </div>
              <div>
                <h3 class="text-sm font-medium text-gray-900">
                  Customer Service
                </h3>
                <ul role="list" class="mt-6 space-y-6">
                  <li v-for="item in footerNavigation.customerService" :key="item.name" class="text-sm">
                    <a :href="item.href" class="text-gray-500 hover:text-gray-600">{{ item.name }}</a>
                  </li>
                </ul>
              </div>
            </div>

            <!-- Newsletter section -->
            <div
              class="mt-12 lg:col-span-4 md:col-span-8 lg:col-start-9 lg:row-start-1 md:col-start-3 md:row-start-2 md:mt-0"
            >
              <h3 class="text-sm font-medium text-gray-900">
                Sign up for our newsletter
              </h3>
              <p class="mt-6 text-sm text-gray-500">
                The latest deals and savings, sent to your inbox weekly.
              </p>
              <form class="mt-2 flex sm:max-w-md">
                <label for="email-address" class="sr-only">Email address</label>
                <input
                  id="email-address" type="text" autocomplete="email" required=""
                  class="min-w-0 w-full appearance-none border border-gray-300 rounded-md bg-white px-4 py-2 text-base text-gray-900 shadow-sm focus:border-indigo-500 focus:outline-none focus:ring-1 focus:ring-indigo-500 placeholder-gray-500"
                >
                <div class="ml-4 flex-shrink-0">
                  <button
                    type="submit"
                    class="w-full flex items-center justify-center border border-transparent rounded-md bg-indigo-600 px-4 py-2 text-base font-medium text-white shadow-sm hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500"
                  >
                    Sign
                    up
                  </button>
                </div>
              </form>
            </div>
          </div>
        </div>

        <div class="border-t border-gray-100 py-10 text-center">
          <p class="text-sm text-gray-500">
            &copy; 2021 Your Company, Inc. All rights reserved.
          </p>
        </div>
      </div>
    </footer>
  </div>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>
