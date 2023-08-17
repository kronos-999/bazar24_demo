<script setup>
import { StarIcon } from '@heroicons/vue/20/solid'

const reviews = {
  average: 4,
  totalCount: 1624,
  counts: [
    { rating: 5, count: 1019 },
    { rating: 4, count: 162 },
    { rating: 3, count: 97 },
    { rating: 2, count: 199 },
    { rating: 1, count: 147 },
  ],
  featured: [
    {
      id: 1,
      rating: 5,
      content: `
        <p>This is the bag of my dreams. I took it on my last vacation and was able to fit an absurd amount of snacks for the many long and hungry flights.</p>
      `,
      author: 'Emily Selman',
      avatarSrc:
        'https://images.unsplash.com/photo-1502685104226-ee32379fefbe?ixlib=rb-=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=8&w=256&h=256&q=80',
    },
    // More reviews...
  ],
}
</script>

<template>
  <div class="bg-white">
    <div
      class="mx-auto max-w-2xl px-4 py-16 lg:grid lg:grid-cols-12 lg:max-w-7xl lg:gap-x-8 lg:px-8 lg:py-32 sm:px-6 sm:py-24"
    >
      <div class="lg:col-span-4">
        <h2 class="text-2xl font-bold tracking-tight text-gray-900">
          Customer Reviews
        </h2>

        <div class="mt-3 flex items-center">
          <div>
            <div class="flex items-center">
              <StarIcon
                v-for="rating in [0, 1, 2, 3, 4]" :key="rating"
                class="h-5 w-5 flex-shrink-0" :class="[reviews.average > rating ? 'text-yellow-400' : 'text-gray-300']"
                aria-hidden="true"
              />
            </div>
            <p class="sr-only">
              {{ reviews.average }} out of 5 stars
            </p>
          </div>
          <p class="ml-2 text-sm text-gray-900">
            Based on {{ reviews.totalCount }} reviews
          </p>
        </div>

        <div class="mt-6">
          <h3 class="sr-only">
            Review data
          </h3>

          <dl class="space-y-3">
            <div v-for="count in reviews.counts" :key="count.rating" class="flex items-center text-sm">
              <dt class="flex flex-1 items-center">
                <p class="w-3 font-medium text-gray-900">
                  {{ count.rating }}<span class="sr-only"> star reviews</span>
                </p>
                <div aria-hidden="true" class="ml-1 flex flex-1 items-center">
                  <StarIcon
                    class="h-5 w-5 flex-shrink-0" :class="[count.count > 0 ? 'text-yellow-400' : 'text-gray-300']"
                    aria-hidden="true"
                  />

                  <div class="relative ml-3 flex-1">
                    <div class="h-3 border border-gray-200 rounded-full bg-gray-100" />
                    <div
                      v-if="count.count > 0"
                      class="absolute inset-y-0 border border-yellow-400 rounded-full bg-yellow-400"
                      :style="{ width: `calc(${count.count} / ${reviews.totalCount} * 100%)` }"
                    />
                  </div>
                </div>
              </dt>
              <dd class="ml-3 w-10 text-right text-sm tabular-nums text-gray-900">
                {{ Math.round((count.count / reviews.totalCount) * 100) }}%
              </dd>
            </div>
          </dl>
        </div>

        <div class="mt-10">
          <h3 class="text-lg font-medium text-gray-900">
            Share your thoughts
          </h3>
          <p class="mt-1 text-sm text-gray-600">
            If you’ve used this product, share your thoughts with other customers
          </p>

          <a
            href="#"
            class="mt-6 w-full inline-flex items-center justify-center border border-gray-300 rounded-md bg-white px-8 py-2 text-sm font-medium text-gray-900 lg:w-full sm:w-auto hover:bg-gray-50"
          >Write
            a review</a>
        </div>
      </div>

      <div class="mt-16 lg:col-span-7 lg:col-start-6 lg:mt-0">
        <h3 class="sr-only">
          Recent reviews
        </h3>

        <div class="flow-root">
          <div class="-my-12 divide-y divide-gray-200">
            <div v-for="review in reviews.featured" :key="review.id" class="py-12">
              <div class="flex items-center">
                <img :src="review.avatarSrc" :alt="`${review.author}.`" class="h-12 w-12 rounded-full">
                <div class="ml-4">
                  <h4 class="text-sm font-bold text-gray-900">
                    {{ review.author }}
                  </h4>
                  <div class="mt-1 flex items-center">
                    <StarIcon
                      v-for="rating in [0, 1, 2, 3, 4]" :key="rating"
                      class="h-5 w-5 flex-shrink-0" :class="[review.rating > rating ? 'text-yellow-400' : 'text-gray-300']"
                      aria-hidden="true"
                    />
                  </div>
                  <p class="sr-only">
                    {{ review.rating }} out of 5 stars
                  </p>
                </div>
              </div>

              <div class="mt-4 text-base italic text-gray-600 space-y-6" v-html="review.content" />
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
