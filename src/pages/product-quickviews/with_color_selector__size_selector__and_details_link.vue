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
import { ref } from 'vue'
import {
  Dialog,
  DialogPanel,
  RadioGroup,
  RadioGroupLabel,
  RadioGroupOption,
  TransitionChild,
  TransitionRoot,
} from '@headlessui/vue'
import { XMarkIcon } from '@heroicons/vue/24/outline'
import { StarIcon } from '@heroicons/vue/20/solid'

const product = {
  name: 'Women\'s Basic Tee',
  price: '$32',
  rating: 3.9,
  reviewCount: 512,
  href: '#',
  imageSrc: 'https://tailwindui.com/img/ecommerce-images/product-page-01-featured-product-shot.jpg',
  imageAlt: 'Back of women\'s Basic Tee in black.',
  colors: [
    { name: 'Black', bgColor: 'bg-gray-900', selectedColor: 'ring-gray-900' },
    { name: 'Heather Grey', bgColor: 'bg-gray-400', selectedColor: 'ring-gray-400' },
  ],
  sizes: [
    { name: 'XXS', inStock: true },
    { name: 'XS', inStock: true },
    { name: 'S', inStock: true },
    { name: 'M', inStock: true },
    { name: 'L', inStock: true },
    { name: 'XL', inStock: true },
    { name: 'XXL', inStock: false },
  ],
}

const open = ref(false)
const selectedColor = ref(product.colors[0])
const selectedSize = ref(product.sizes[2])
</script>

<template>
  <TransitionRoot as="template" :show="open">
    <Dialog as="div" class="relative z-10" @close="open = false">
      <TransitionChild as="template" enter="ease-out duration-300" enter-from="opacity-0" enter-to="opacity-100" leave="ease-in duration-200" leave-from="opacity-100" leave-to="opacity-0">
        <div class="fixed inset-0 hidden bg-gray-500 bg-opacity-75 transition-opacity md:block" />
      </TransitionChild>

      <div class="fixed inset-0 z-10 overflow-y-auto">
        <div class="min-h-full flex items-stretch justify-center text-center md:items-center lg:px-4 md:px-2">
          <!-- This element is to trick the browser into centering the modal contents. -->
          <span class="hidden md:inline-block md:h-screen md:align-middle" aria-hidden="true">&#8203;</span>
          <TransitionChild as="template" enter="ease-out duration-300" enter-from="opacity-0 translate-y-4 md:translate-y-0 md:scale-95" enter-to="opacity-100 translate-y-0 md:scale-100" leave="ease-in duration-200" leave-from="opacity-100 translate-y-0 md:scale-100" leave-to="opacity-0 translate-y-4 md:translate-y-0 md:scale-95">
            <DialogPanel class="w-full flex transform text-left text-base transition md:my-8 lg:max-w-4xl md:max-w-2xl md:px-4">
              <div class="relative w-full flex items-center overflow-hidden bg-white px-4 pb-8 pt-14 shadow-2xl lg:p-8 md:p-6 sm:px-6 sm:pt-8">
                <button type="button" class="absolute right-4 top-4 text-gray-400 lg:right-8 lg:top-8 md:right-6 md:top-6 sm:right-6 sm:top-8 hover:text-gray-500" @click="open = false">
                  <span class="sr-only">Close</span>
                  <XMarkIcon class="h-6 w-6" aria-hidden="true" />
                </button>

                <div class="grid grid-cols-1 w-full items-start gap-x-6 gap-y-8 sm:grid-cols-12 lg:items-center lg:gap-x-8">
                  <div class="aspect-w-2 aspect-h-3 overflow-hidden rounded-lg bg-gray-100 lg:col-span-5 sm:col-span-4">
                    <img :src="product.imageSrc" :alt="product.imageAlt" class="object-cover object-center">
                  </div>
                  <div class="lg:col-span-7 sm:col-span-8">
                    <h2 class="text-xl font-medium text-gray-900 sm:pr-12">
                      {{ product.name }}
                    </h2>

                    <section aria-labelledby="information-heading" class="mt-1">
                      <h3 id="information-heading" class="sr-only">
                        Product information
                      </h3>

                      <p class="font-medium text-gray-900">
                        {{ product.price }}
                      </p>

                      <!-- Reviews -->
                      <div class="mt-4">
                        <h4 class="sr-only">
                          Reviews
                        </h4>
                        <div class="flex items-center">
                          <p class="text-sm text-gray-700">
                            {{ product.rating }}
                            <span class="sr-only"> out of 5 stars</span>
                          </p>
                          <div class="ml-1 flex items-center">
                            <StarIcon v-for="rating in [0, 1, 2, 3, 4]" :key="rating" class="h-5 w-5 flex-shrink-0" :class="[product.rating > rating ? 'text-yellow-400' : 'text-gray-200']" aria-hidden="true" />
                          </div>
                          <div class="ml-4 hidden lg:flex lg:items-center">
                            <span class="text-gray-300" aria-hidden="true">&middot;</span>
                            <a href="#" class="ml-4 text-sm font-medium text-indigo-600 hover:text-indigo-500">See all {{ product.reviewCount }} reviews</a>
                          </div>
                        </div>
                      </div>
                    </section>

                    <section aria-labelledby="options-heading" class="mt-8">
                      <h3 id="options-heading" class="sr-only">
                        Product options
                      </h3>

                      <form>
                        <!-- Color picker -->
                        <div>
                          <h4 class="text-sm font-medium text-gray-900">
                            Color
                          </h4>

                          <RadioGroup v-model="selectedColor" class="mt-2">
                            <RadioGroupLabel class="sr-only">
                              Choose a color
                            </RadioGroupLabel>
                            <div class="flex items-center space-x-3">
                              <RadioGroupOption v-for="color in product.colors" :key="color.name" v-slot="{ active, checked }" as="template" :value="color">
                                <div class="relative flex cursor-pointer items-center justify-center rounded-full p-0.5 -m-0.5 focus:outline-none" :class="[color.selectedColor, active && checked ? 'ring ring-offset-1' : '', !active && checked ? 'ring-2' : '']">
                                  <RadioGroupLabel as="span" class="sr-only">
                                    {{ color.name }}
                                  </RadioGroupLabel>
                                  <span aria-hidden="true" class="h-8 w-8 border border-black border-opacity-10 rounded-full" :class="[color.bgColor]" />
                                </div>
                              </RadioGroupOption>
                            </div>
                          </RadioGroup>
                        </div>

                        <!-- Size picker -->
                        <div class="mt-8">
                          <div class="flex items-center justify-between">
                            <h4 class="text-sm font-medium text-gray-900">
                              Size
                            </h4>
                            <a href="#" class="text-sm font-medium text-indigo-600 hover:text-indigo-500">Size guide</a>
                          </div>

                          <RadioGroup v-model="selectedSize" class="mt-2">
                            <RadioGroupLabel class="sr-only">
                              Choose a size
                            </RadioGroupLabel>
                            <div class="grid grid-cols-7 gap-2">
                              <RadioGroupOption v-for="size in product.sizes" :key="size.name" v-slot="{ active, checked }" as="template" :value="size" :disabled="!size.inStock">
                                <div class="flex items-center justify-center border rounded-md px-3 py-3 text-sm font-medium uppercase sm:flex-1" :class="[size.inStock ? 'cursor-pointer focus:outline-none' : 'opacity-25 cursor-not-allowed', active ? 'ring-2 ring-offset-2 ring-indigo-500' : '', checked ? 'bg-indigo-600 border-transparent text-white hover:bg-indigo-700' : 'bg-white border-gray-200 text-gray-900 hover:bg-gray-50']">
                                  <RadioGroupLabel as="span">
                                    {{ size.name }}
                                  </RadioGroupLabel>
                                </div>
                              </RadioGroupOption>
                            </div>
                          </RadioGroup>
                        </div>

                        <button type="submit" class="mt-8 w-full flex items-center justify-center border border-transparent rounded-md bg-indigo-600 px-8 py-3 text-base font-medium text-white hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500">
                          Add to bag
                        </button>

                        <p class="absolute left-4 top-4 text-center sm:static sm:mt-8">
                          <a :href="product.href" class="font-medium text-indigo-600 hover:text-indigo-500">View full details</a>
                        </p>
                      </form>
                    </section>
                  </div>
                </div>
              </div>
            </DialogPanel>
          </TransitionChild>
        </div>
      </div>
    </Dialog>
  </TransitionRoot>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>
