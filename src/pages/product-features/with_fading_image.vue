<script setup>
const features = [
  { name: 'Origin', description: 'Designed by Good Goods, Inc.' },
  { name: 'Material', description: 'Solid walnut base with rare earth magnets and polycarbonate add-ons.' },
  { name: 'Dimensions', description: '15" x 3.75" x .75"' },
  { name: 'Finish', description: 'Hand sanded and finished with natural oil' },
  { name: 'Includes', description: 'Pen Tray, Phone Tray, Small Tray, Large Tray, Sticky Note Holder' },
  { name: 'Considerations', description: 'Made from natural materials. Grain and color vary with each item.' },
]
</script>

<template>
  <div class="bg-white">
    <div aria-hidden="true" class="relative">
      <img
        src="https://tailwindui.com/img/ecommerce-images/product-feature-02-full-width.jpg" alt=""
        class="h-96 w-full object-cover object-center"
      >
      <div class="absolute inset-0 from-white bg-gradient-to-t" />
    </div>

    <div class="relative mx-auto max-w-7xl px-4 pb-16 -mt-12 lg:px-8 sm:px-6 sm:pb-24">
      <div class="mx-auto max-w-2xl text-center lg:max-w-4xl">
        <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">
          Technical Specifications
        </h2>
        <p class="mt-4 text-gray-500">
          Organize is a system to keep your desk tidy and photo-worthy all day long.
          Procrastinate your work while you meticulously arrange items into dedicated trays.
        </p>
      </div>

      <dl
        class="grid grid-cols-1 mx-auto mt-16 max-w-2xl gap-x-6 gap-y-10 lg:grid-cols-3 sm:grid-cols-2 lg:max-w-none lg:gap-x-8 sm:gap-y-16"
      >
        <div v-for="feature in features" :key="feature.name" class="border-t border-gray-200 pt-4">
          <dt class="font-medium text-gray-900">
            {{ feature.name }}
          </dt>
          <dd class="mt-2 text-sm text-gray-500">
            {{ feature.description }}
          </dd>
        </div>
      </dl>
    </div>
  </div>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>
