<!--
  This example requires some changes to your config:

  ```
  // tailwind.config.js
  module.exports = {
    // ...
    plugins: [
      // ...
      require('@tailwindcss/forms'),
    ],
  }
  ```
-->
<script setup>
import { Disclosure, DisclosureButton, DisclosurePanel } from '@headlessui/vue'
import { LockClosedIcon } from '@heroicons/vue/20/solid'

const subtotal = '$210.00'
const discount = { code: 'CHEAPSKATE', amount: '$24.00' }
const taxes = '$23.68'
const shipping = '$22.00'
const total = '$341.68'
const products = [
  {
    id: 1,
    name: 'Micro Backpack',
    href: '#',
    price: '$70.00',
    color: 'Moss',
    size: '5L',
    imageSrc: 'https://tailwindui.com/img/ecommerce-images/checkout-page-04-product-01.jpg',
    imageAlt:
      'Moss green canvas compact backpack with double top zipper, zipper front pouch, and matching carry handle and backpack straps.',
  },
  // More products...
]
</script>

<template>
  <!--
    This example requires updating your template:

    ```
    <html class="h-full bg-white">
    <body class="h-full">
    ```
  -->
  <main class="lg:min-h-full lg:flex lg:flex-row-reverse lg:overflow-hidden">
    <div class="px-4 py-6 lg:hidden sm:px-6">
      <div class="mx-auto max-w-lg flex">
        <a href="#">
          <span class="sr-only">Your Company</span>
          <img src="https://tailwindui.com/img/logos/mark.svg?color=indigo&amp;shade=600" alt="" class="h-8 w-auto">
        </a>
      </div>
    </div>

    <h1 class="sr-only">
      Checkout
    </h1>

    <!-- Mobile order summary -->
    <section aria-labelledby="order-heading" class="bg-gray-50 px-4 py-6 lg:hidden sm:px-6">
      <Disclosure v-slot="{ open }" as="div" class="mx-auto max-w-lg">
        <div class="flex items-center justify-between">
          <h2 id="order-heading" class="text-lg font-medium text-gray-900">
            Your Order
          </h2>
          <DisclosureButton class="font-medium text-indigo-600 hover:text-indigo-500">
            <span v-if="open">Hide full summary</span>
            <span v-if="!open">Show full summary</span>
          </DisclosureButton>
        </div>

        <DisclosurePanel>
          <ul role="list" class="border-b border-gray-200 divide-y divide-gray-200">
            <li v-for="product in products" :key="product.id" class="flex py-6 space-x-6">
              <img
                :src="product.imageSrc" :alt="product.imageAlt"
                class="h-40 w-40 flex-none rounded-md bg-gray-200 object-cover object-center"
              >
              <div class="flex flex-col justify-between space-y-4">
                <div class="text-sm font-medium space-y-1">
                  <h3 class="text-gray-900">
                    {{ product.name }}
                  </h3>
                  <p class="text-gray-900">
                    {{ product.price }}
                  </p>
                  <p class="text-gray-500">
                    {{ product.color }}
                  </p>
                  <p class="text-gray-500">
                    {{ product.size }}
                  </p>
                </div>
                <div class="flex space-x-4">
                  <button type="button" class="text-sm font-medium text-indigo-600 hover:text-indigo-500">
                    Edit
                  </button>
                  <div class="flex border-l border-gray-300 pl-4">
                    <button
                      type="button"
                      class="text-sm font-medium text-indigo-600 hover:text-indigo-500"
                    >
                      Remove
                    </button>
                  </div>
                </div>
              </div>
            </li>
          </ul>

          <form class="mt-10">
            <label for="discount-code-mobile" class="block text-sm font-medium text-gray-700">Discount code</label>
            <div class="mt-1 flex space-x-4">
              <input
                id="discount-code-mobile" type="text" name="discount-code-mobile"
                class="block w-full border-gray-300 rounded-md bg-white px-3 py-2 text-gray-900 shadow-sm focus:border-indigo-500 sm:text-sm focus-visible:outline-none focus:ring-2 focus:ring-indigo-500"
              >
              <button
                type="submit"
                class="rounded-md bg-gray-200 px-4 text-sm font-medium text-gray-600 hover:bg-gray-300 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500 focus:ring-offset-gray-50"
              >
                Apply
              </button>
            </div>
          </form>

          <dl class="mt-10 text-sm font-medium text-gray-500 space-y-6">
            <div class="flex justify-between">
              <dt>Subtotal</dt>
              <dd class="text-gray-900">
                {{ subtotal }}
              </dd>
            </div>
            <div class="flex justify-between">
              <dt class="flex">
                Discount
                <span
                  class="ml-2 rounded-full bg-gray-200 px-2 py-0.5 text-xs tracking-wide text-gray-600"
                >{{ discount.code }}</span>
              </dt>
              <dd class="text-gray-900">
                -{{ discount.amount }}
              </dd>
            </div>
            <div class="flex justify-between">
              <dt>Taxes</dt>
              <dd class="text-gray-900">
                {{ taxes }}
              </dd>
            </div>
            <div class="flex justify-between">
              <dt>Shipping</dt>
              <dd class="text-gray-900">
                {{ shipping }}
              </dd>
            </div>
          </dl>
        </DisclosurePanel>

        <p class="mt-6 flex items-center justify-between border-t border-gray-200 pt-6 text-sm font-medium text-gray-900">
          <span class="text-base">Total</span>
          <span class="text-base">{{ total }}</span>
        </p>
      </Disclosure>
    </section>

    <!-- Order summary -->
    <section aria-labelledby="summary-heading" class="hidden max-w-md w-full flex-col bg-gray-50 lg:flex">
      <h2 id="summary-heading" class="sr-only">
        Order summary
      </h2>

      <ul role="list" class="flex-auto overflow-y-auto px-6 divide-y divide-gray-200">
        <li v-for="product in products" :key="product.id" class="flex py-6 space-x-6">
          <img
            :src="product.imageSrc" :alt="product.imageAlt"
            class="h-40 w-40 flex-none rounded-md bg-gray-200 object-cover object-center"
          >
          <div class="flex flex-col justify-between space-y-4">
            <div class="text-sm font-medium space-y-1">
              <h3 class="text-gray-900">
                {{ product.name }}
              </h3>
              <p class="text-gray-900">
                {{ product.price }}
              </p>
              <p class="text-gray-500">
                {{ product.color }}
              </p>
              <p class="text-gray-500">
                {{ product.size }}
              </p>
            </div>
            <div class="flex space-x-4">
              <button type="button" class="text-sm font-medium text-indigo-600 hover:text-indigo-500">
                Edit
              </button>
              <div class="flex border-l border-gray-300 pl-4">
                <button type="button" class="text-sm font-medium text-indigo-600 hover:text-indigo-500">
                  Remove
                </button>
              </div>
            </div>
          </div>
        </li>
      </ul>

      <div class="sticky bottom-0 flex-none border-t border-gray-200 bg-gray-50 p-6">
        <form>
          <label for="discount-code" class="block text-sm font-medium text-gray-700">Discount code</label>
          <div class="mt-1 flex space-x-4">
            <input
              id="discount-code" type="text" name="discount-code"
              class="block w-full border-gray-300 rounded-md bg-white px-3 py-2 text-gray-900 shadow-sm focus:border-indigo-500 sm:text-sm focus-visible:outline-none focus:ring-2 focus:ring-indigo-500"
            >
            <button
              type="submit"
              class="rounded-md bg-gray-200 px-4 text-sm font-medium text-gray-600 hover:bg-gray-300 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500 focus:ring-offset-gray-50"
            >
              Apply
            </button>
          </div>
        </form>

        <dl class="mt-10 text-sm font-medium text-gray-500 space-y-6">
          <div class="flex justify-between">
            <dt>Subtotal</dt>
            <dd class="text-gray-900">
              {{ subtotal }}
            </dd>
          </div>
          <div class="flex justify-between">
            <dt class="flex">
              Discount
              <span
                class="ml-2 rounded-full bg-gray-200 px-2 py-0.5 text-xs tracking-wide text-gray-600"
              >{{ discount.code }}</span>
            </dt>
            <dd class="text-gray-900">
              -{{ discount.amount }}
            </dd>
          </div>
          <div class="flex justify-between">
            <dt>Taxes</dt>
            <dd class="text-gray-900">
              {{ taxes }}
            </dd>
          </div>
          <div class="flex justify-between">
            <dt>Shipping</dt>
            <dd class="text-gray-900">
              {{ shipping }}
            </dd>
          </div>
          <div class="flex items-center justify-between border-t border-gray-200 pt-6 text-gray-900">
            <dt class="text-base">
              Total
            </dt>
            <dd class="text-base">
              {{ total }}
            </dd>
          </div>
        </dl>
      </div>
    </section>

    <!-- Checkout form -->
    <section
      aria-labelledby="payment-heading"
      class="flex-auto overflow-y-auto px-4 pb-16 pt-12 lg:px-8 sm:px-6 lg:pb-24 lg:pt-0 sm:pt-16"
    >
      <div class="mx-auto max-w-lg">
        <div class="hidden pb-16 pt-10 lg:flex">
          <a href="#">
            <span class="sr-only">Your Company</span>
            <img src="https://tailwindui.com/img/logos/mark.svg?color=indigo&amp;shade=600" alt="" class="h-8 w-auto">
          </a>
        </div>

        <button
          type="button"
          class="w-full flex items-center justify-center border border-transparent rounded-md bg-black py-2 text-white hover:bg-gray-800 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-gray-900"
        >
          <span class="sr-only">Pay with Apple Pay</span>
          <svg class="h-5 w-auto" fill="currentColor" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 50 20">
            <path
              d="M9.536 2.579c-.571.675-1.485 1.208-2.4 1.132-.113-.914.334-1.884.858-2.484C8.565.533 9.564.038 10.374 0c.095.951-.276 1.884-.838 2.579zm.829 1.313c-1.324-.077-2.457.751-3.085.751-.638 0-1.6-.713-2.647-.694-1.362.019-2.628.79-3.323 2.017-1.429 2.455-.372 6.09 1.009 8.087.676.99 1.485 2.075 2.552 2.036 1.009-.038 1.409-.656 2.628-.656 1.228 0 1.58.656 2.647.637 1.104-.019 1.8-.99 2.475-1.979.771-1.122 1.086-2.217 1.105-2.274-.02-.019-2.133-.828-2.152-3.263-.02-2.036 1.666-3.007 1.742-3.064-.952-1.408-2.437-1.56-2.951-1.598zm7.645-2.76v14.834h2.305v-5.072h3.19c2.913 0 4.96-1.998 4.96-4.89 0-2.893-2.01-4.872-4.885-4.872h-5.57zm2.305 1.941h2.656c2 0 3.142 1.066 3.142 2.94 0 1.875-1.142 2.95-3.151 2.95h-2.647v-5.89zM32.673 16.08c1.448 0 2.79-.733 3.4-1.893h.047v1.779h2.133V8.582c0-2.14-1.714-3.52-4.351-3.52-2.447 0-4.256 1.399-4.323 3.32h2.076c.171-.913 1.018-1.512 2.18-1.512 1.41 0 2.2.656 2.2 1.865v.818l-2.876.171c-2.675.162-4.123 1.256-4.123 3.159 0 1.922 1.495 3.197 3.637 3.197zm.62-1.76c-1.229 0-2.01-.59-2.01-1.494 0-.933.752-1.475 2.19-1.56l2.562-.162v.837c0 1.39-1.181 2.379-2.743 2.379zM41.1 20c2.247 0 3.304-.856 4.227-3.454l4.047-11.341h-2.342l-2.714 8.763h-.047l-2.714-8.763h-2.409l3.904 10.799-.21.656c-.352 1.114-.923 1.542-1.942 1.542-.18 0-.533-.02-.676-.038v1.779c.133.038.705.057.876.057z"
            />
          </svg>
        </button>

        <div class="relative mt-8">
          <div class="absolute inset-0 flex items-center" aria-hidden="true">
            <div class="w-full border-t border-gray-200" />
          </div>
          <div class="relative flex justify-center">
            <span class="bg-white px-4 text-sm font-medium text-gray-500">or</span>
          </div>
        </div>

        <form class="mt-6">
          <div class="grid grid-cols-12 gap-x-4 gap-y-6">
            <div class="col-span-full">
              <label for="email-address" class="block text-sm font-medium text-gray-700">Email address</label>
              <div class="mt-1">
                <input
                  id="email-address" type="email" name="email-address" autocomplete="email"
                  class="block w-full border-gray-300 rounded-md bg-white px-3 py-2 text-gray-900 shadow-sm focus:border-indigo-500 sm:text-sm focus-visible:outline-none focus:ring-2 focus:ring-indigo-500"
                >
              </div>
            </div>

            <div class="col-span-full">
              <label for="name-on-card" class="block text-sm font-medium text-gray-700">Name on card</label>
              <div class="mt-1">
                <input
                  id="name-on-card" type="text" name="name-on-card" autocomplete="cc-name"
                  class="block w-full border-gray-300 rounded-md bg-white px-3 py-2 text-gray-900 shadow-sm focus:border-indigo-500 sm:text-sm focus-visible:outline-none focus:ring-2 focus:ring-indigo-500"
                >
              </div>
            </div>

            <div class="col-span-full">
              <label for="card-number" class="block text-sm font-medium text-gray-700">Card number</label>
              <div class="mt-1">
                <input
                  id="card-number" type="text" name="card-number" autocomplete="cc-number"
                  class="block w-full border-gray-300 rounded-md bg-white px-3 py-2 text-gray-900 shadow-sm focus:border-indigo-500 sm:text-sm focus-visible:outline-none focus:ring-2 focus:ring-indigo-500"
                >
              </div>
            </div>

            <div class="col-span-8 sm:col-span-9">
              <label for="expiration-date" class="block text-sm font-medium text-gray-700">Expiration date (MM/YY)</label>
              <div class="mt-1">
                <input
                  id="expiration-date" type="text" name="expiration-date" autocomplete="cc-exp"
                  class="block w-full border-gray-300 rounded-md bg-white px-3 py-2 text-gray-900 shadow-sm focus:border-indigo-500 sm:text-sm focus-visible:outline-none focus:ring-2 focus:ring-indigo-500"
                >
              </div>
            </div>

            <div class="col-span-4 sm:col-span-3">
              <label for="cvc" class="block text-sm font-medium text-gray-700">CVC</label>
              <div class="mt-1">
                <input
                  id="cvc" type="text" name="cvc" autocomplete="csc"
                  class="block w-full border-gray-300 rounded-md bg-white px-3 py-2 text-gray-900 shadow-sm focus:border-indigo-500 sm:text-sm focus-visible:outline-none focus:ring-2 focus:ring-indigo-500"
                >
              </div>
            </div>

            <div class="col-span-full">
              <label for="address" class="block text-sm font-medium text-gray-700">Address</label>
              <div class="mt-1">
                <input
                  id="address" type="text" name="address" autocomplete="street-address"
                  class="block w-full border-gray-300 rounded-md bg-white px-3 py-2 text-gray-900 shadow-sm focus:border-indigo-500 sm:text-sm focus-visible:outline-none focus:ring-2 focus:ring-indigo-500"
                >
              </div>
            </div>

            <div class="col-span-full sm:col-span-4">
              <label for="city" class="block text-sm font-medium text-gray-700">City</label>
              <div class="mt-1">
                <input
                  id="city" type="text" name="city" autocomplete="address-level2"
                  class="block w-full border-gray-300 rounded-md bg-white px-3 py-2 text-gray-900 shadow-sm focus:border-indigo-500 sm:text-sm focus-visible:outline-none focus:ring-2 focus:ring-indigo-500"
                >
              </div>
            </div>

            <div class="col-span-full sm:col-span-4">
              <label for="region" class="block text-sm font-medium text-gray-700">State / Province</label>
              <div class="mt-1">
                <input
                  id="region" type="text" name="region" autocomplete="address-level1"
                  class="block w-full border-gray-300 rounded-md bg-white px-3 py-2 text-gray-900 shadow-sm focus:border-indigo-500 sm:text-sm focus-visible:outline-none focus:ring-2 focus:ring-indigo-500"
                >
              </div>
            </div>

            <div class="col-span-full sm:col-span-4">
              <label for="postal-code" class="block text-sm font-medium text-gray-700">Postal code</label>
              <div class="mt-1">
                <input
                  id="postal-code" type="text" name="postal-code" autocomplete="postal-code"
                  class="block w-full border-gray-300 rounded-md bg-white px-3 py-2 text-gray-900 shadow-sm focus:border-indigo-500 sm:text-sm focus-visible:outline-none focus:ring-2 focus:ring-indigo-500"
                >
              </div>
            </div>
          </div>

          <div class="mt-6 flex space-x-2">
            <div class="h-5 flex items-center">
              <input
                id="same-as-shipping" name="same-as-shipping" type="checkbox" checked=""
                class="h-4 w-4 border-gray-300 rounded text-indigo-600 focus:ring-indigo-500"
              >
            </div>
            <label for="same-as-shipping" class="text-sm font-medium text-gray-900">Billing address is the same as
              shipping address</label>
          </div>

          <button
            type="submit"
            class="mt-6 w-full border border-transparent rounded-md bg-indigo-600 px-4 py-2 text-sm font-medium text-white shadow-sm hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500"
          >
            Pay
            {{ total }}
          </button>

          <p class="mt-6 flex justify-center text-sm font-medium text-gray-500">
            <LockClosedIcon class="mr-1.5 h-5 w-5 text-gray-400" aria-hidden="true" />
            Payment details stored in plain text
          </p>
        </form>
      </div>
    </section>
  </main>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>
