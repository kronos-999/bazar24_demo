<script>
export default {
  props: {
    theme: {
      type: String,
      default: 'red',
    },
  },
}
</script>

<template>
  <footer class="body-font text-gray-600 dark:bg-gray-900 dark:text-gray-400">
    <div
      class="mx-auto flex flex-col flex-wrap px-5 py-24 container md:flex-row md:flex-nowrap lg:items-start md:items-center"
    >
      <div class="mx-auto mt-10 w-64 flex-shrink-0 text-center md:mx-0 md:mt-0 md:text-left">
        <a
          class="title-font flex items-center justify-center font-medium text-gray-900 md:justify-start dark:text-white"
        >
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            :class="`w-10 h-10 text-white p-2 bg-${theme}-500 rounded-full`"
            viewBox="0 0 24 24"
          >
            <path d="M12 2L2 7l10 5 10-5-10-5zM2 17l10 5 10-5M2 12l10 5 10-5" />
          </svg>
          <span class="ml-3 text-xl">Tailblocks</span>
        </a>
        <p class="mt-2 text-sm text-gray-500">
          Air plant banjo lyft occupy retro adaptogen indego
        </p>
      </div>
      <div class="order-first flex flex-grow flex-wrap text-center -mb-10 md:pr-20 md:text-left">
        <div class="w-full px-4 lg:w-1/4 md:w-1/2">
          <h2 class="title-font mb-3 text-sm font-medium tracking-widest text-gray-900 dark:text-white">
            CATEGORIES
          </h2>
          <nav class="mb-10 list-none">
            <li>
              <a class="text-gray-600 dark:text-gray-400 hover:text-gray-800 dark:hover:text-white">First Link</a>
            </li>
            <li>
              <a class="text-gray-600 dark:text-gray-400 hover:text-gray-800 dark:hover:text-white">Second Link</a>
            </li>
            <li>
              <a class="text-gray-600 dark:text-gray-400 hover:text-gray-800 dark:hover:text-white">Third Link</a>
            </li>
            <li>
              <a class="text-gray-600 dark:text-gray-400 hover:text-gray-800 dark:hover:text-white">Fourth Link</a>
            </li>
          </nav>
        </div>
        <div class="w-full px-4 lg:w-1/4 md:w-1/2">
          <h2 class="title-font mb-3 text-sm font-medium tracking-widest text-gray-900 dark:text-white">
            CATEGORIES
          </h2>
          <nav class="mb-10 list-none">
            <li>
              <a class="text-gray-600 dark:text-gray-400 hover:text-gray-800 dark:hover:text-white">First Link</a>
            </li>
            <li>
              <a class="text-gray-600 dark:text-gray-400 hover:text-gray-800 dark:hover:text-white">Second Link</a>
            </li>
            <li>
              <a class="text-gray-600 dark:text-gray-400 hover:text-gray-800 dark:hover:text-white">Third Link</a>
            </li>
            <li>
              <a class="text-gray-600 dark:text-gray-400 hover:text-gray-800 dark:hover:text-white">Fourth Link</a>
            </li>
          </nav>
        </div>
        <div class="w-full px-4 lg:w-1/4 md:w-1/2">
          <h2 class="title-font mb-3 text-sm font-medium tracking-widest text-gray-900 dark:text-white">
            CATEGORIES
          </h2>
          <nav class="mb-10 list-none">
            <li>
              <a class="text-gray-600 dark:text-gray-400 hover:text-gray-800 dark:hover:text-white">First Link</a>
            </li>
            <li>
              <a class="text-gray-600 dark:text-gray-400 hover:text-gray-800 dark:hover:text-white">Second Link</a>
            </li>
            <li>
              <a class="text-gray-600 dark:text-gray-400 hover:text-gray-800 dark:hover:text-white">Third Link</a>
            </li>
            <li>
              <a class="text-gray-600 dark:text-gray-400 hover:text-gray-800 dark:hover:text-white">Fourth Link</a>
            </li>
          </nav>
        </div>
        <div class="w-full px-4 lg:w-1/4 md:w-1/2">
          <h2 class="title-font mb-3 text-sm font-medium tracking-widest text-gray-900 dark:text-white">
            CATEGORIES
          </h2>
          <nav class="mb-10 list-none">
            <li>
              <a class="text-gray-600 dark:text-gray-400 hover:text-gray-800 dark:hover:text-white">First Link</a>
            </li>
            <li>
              <a class="text-gray-600 dark:text-gray-400 hover:text-gray-800 dark:hover:text-white">Second Link</a>
            </li>
            <li>
              <a class="text-gray-600 dark:text-gray-400 hover:text-gray-800 dark:hover:text-white">Third Link</a>
            </li>
            <li>
              <a class="text-gray-600 dark:text-gray-400 hover:text-gray-800 dark:hover:text-white">Fourth Link</a>
            </li>
          </nav>
        </div>
      </div>
    </div>
    <div class="bg-gray-100 dark:bg-gray-800 dark:bg-opacity-75">
      <div class="mx-auto flex flex-col flex-wrap px-5 py-4 container sm:flex-row">
        <p class="text-center text-sm text-gray-500 sm:text-left dark:text-gray-400">
          © 2020 Tailblocks —
          <a
            href="https://twitter.com/knyttneve"
            rel="noopener noreferrer"
            class="ml-1 text-gray-600 dark:text-gray-500"
            target="_blank"
          >@knyttneve</a>
        </p>
        <span class="mt-2 inline-flex justify-center sm:ml-auto sm:mt-0 sm:justify-start">
          <a class="text-gray-500 dark:text-gray-400">
            <svg
              fill="currentColor"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              class="h-5 w-5"
              viewBox="0 0 24 24"
            >
              <path d="M18 2h-3a5 5 0 00-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 011-1h3z" />
            </svg>
          </a>
          <a class="ml-3 text-gray-500 dark:text-gray-400">
            <svg
              fill="currentColor"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              class="h-5 w-5"
              viewBox="0 0 24 24"
            >
              <path
                d="M23 3a10.9 10.9 0 01-3.14 1.53 4.48 4.48 0 00-7.86 3v1A10.66 10.66 0 013 4s-4 9 5 13a11.64 11.64 0 01-7 2c9 5 20 0 20-11.5a4.5 4.5 0 00-.08-.83A7.72 7.72 0 0023 3z"
              />
            </svg>
          </a>
          <a class="ml-3 text-gray-500 dark:text-gray-400">
            <svg
              fill="none"
              stroke="currentColor"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              class="h-5 w-5"
              viewBox="0 0 24 24"
            >
              <rect width="20" height="20" x="2" y="2" rx="5" ry="5" />
              <path d="M16 11.37A4 4 0 1112.63 8 4 4 0 0116 11.37zm1.5-4.87h.01" />
            </svg>
          </a>
          <a class="ml-3 text-gray-500 dark:text-gray-400">
            <svg
              fill="currentColor"
              stroke="currentColor"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="0"
              class="h-5 w-5"
              viewBox="0 0 24 24"
            >
              <path
                stroke="none"
                d="M16 8a6 6 0 016 6v7h-4v-7a2 2 0 00-2-2 2 2 0 00-2 2v7h-4v-7a6 6 0 016-6zM2 9h4v12H2z"
              />
              <circle cx="4" cy="4" r="2" stroke="none" />
            </svg>
          </a>
        </span>
      </div>
    </div>
  </footer>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>

<style></style>
