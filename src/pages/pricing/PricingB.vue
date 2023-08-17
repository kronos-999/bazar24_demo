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
  <section class="body-font text-gray-600 dark:bg-gray-900 dark:text-gray-400">
    <div class="mx-auto px-5 py-24 container">
      <div class="mb-20 w-full flex flex-col text-center">
        <h1 class="title-font mb-2 text-3xl font-medium text-gray-900 sm:text-4xl dark:text-white">
          Pricing
        </h1>
        <p class="mx-auto text-base leading-relaxed lg:w-2/3">
          Banh mi cornhole echo park skateboard authentic crucifix neutra tilde lyft biodiesel artisan direct trade
          mumblecore 3 wolf moon twee
        </p>
      </div>
      <div class="mx-auto w-full overflow-auto lg:w-2/3">
        <table class="whitespace-no-wrap w-full table-auto text-left">
          <thead>
            <tr>
              <th
                class="title-font rounded-bl rounded-tl bg-gray-100 px-4 py-3 text-sm font-medium tracking-wider text-gray-900 dark:bg-gray-800 dark:text-white"
              >
                Plan
              </th>
              <th
                class="title-font bg-gray-100 px-4 py-3 text-sm font-medium tracking-wider text-gray-900 dark:bg-gray-800 dark:text-white"
              >
                Speed
              </th>
              <th
                class="title-font bg-gray-100 px-4 py-3 text-sm font-medium tracking-wider text-gray-900 dark:bg-gray-800 dark:text-white"
              >
                Storage
              </th>
              <th
                class="title-font bg-gray-100 px-4 py-3 text-sm font-medium tracking-wider text-gray-900 dark:bg-gray-800 dark:text-white"
              >
                Price
              </th>
              <th
                class="title-font w-10 rounded-br rounded-tr bg-gray-100 text-sm font-medium tracking-wider text-gray-900 dark:bg-gray-800 dark:text-white"
              />
            </tr>
          </thead>
          <tbody>
            <tr>
              <td class="px-4 py-3">
                Start
              </td>
              <td class="px-4 py-3">
                5 Mb/s
              </td>
              <td class="px-4 py-3">
                15 GB
              </td>
              <td class="px-4 py-3 text-lg text-gray-900 dark:text-white">
                Free
              </td>
              <td class="w-10 text-center">
                <input name="plan" type="radio">
              </td>
            </tr>
            <tr>
              <td class="border-t-2 border-gray-200 px-4 py-3 dark:border-gray-800">
                Pro
              </td>
              <td class="border-t-2 border-gray-200 px-4 py-3 dark:border-gray-800">
                25 Mb/s
              </td>
              <td class="border-t-2 border-gray-200 px-4 py-3 dark:border-gray-800">
                25 GB
              </td>
              <td class="border-t-2 border-gray-200 px-4 py-3 text-lg text-gray-900 dark:border-gray-800 dark:text-white">
                $24
              </td>
              <td class="w-10 border-t-2 border-gray-200 text-center dark:border-gray-800">
                <input name="plan" type="radio">
              </td>
            </tr>
            <tr>
              <td class="border-t-2 border-gray-200 px-4 py-3 dark:border-gray-800">
                Business
              </td>
              <td class="border-t-2 border-gray-200 px-4 py-3 dark:border-gray-800">
                36 Mb/s
              </td>
              <td class="border-t-2 border-gray-200 px-4 py-3 dark:border-gray-800">
                40 GB
              </td>
              <td class="border-t-2 border-gray-200 px-4 py-3 text-lg text-gray-900 dark:border-gray-800 dark:text-white">
                $50
              </td>
              <td class="w-10 border-t-2 border-gray-200 text-center dark:border-gray-800">
                <input name="plan" type="radio">
              </td>
            </tr>
            <tr>
              <td class="border-b-2 border-t-2 border-gray-200 px-4 py-3 dark:border-gray-800">
                Exclusive
              </td>
              <td class="border-b-2 border-t-2 border-gray-200 px-4 py-3 dark:border-gray-800">
                48 Mb/s
              </td>
              <td class="border-b-2 border-t-2 border-gray-200 px-4 py-3 dark:border-gray-800">
                120 GB
              </td>
              <td
                class="border-b-2 border-t-2 border-gray-200 px-4 py-3 text-lg text-gray-900 dark:border-gray-800 dark:text-white"
              >
                $72
              </td>
              <td class="w-10 border-b-2 border-t-2 border-gray-200 text-center dark:border-gray-800">
                <input name="plan" type="radio">
              </td>
            </tr>
          </tbody>
        </table>
      </div>
      <div class="mx-auto mt-4 w-full flex pl-4 lg:w-2/3">
        <a :class="`text-${theme}-500 inline-flex items-center md:mb-2 lg:mb-0 dark:text-${theme}-400`">Learn More
          <svg
            fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
            class="ml-2 h-4 w-4" viewBox="0 0 24 24"
          >
            <path d="M5 12h14M12 5l7 7-7 7" />
          </svg>
        </a>
        <button
          :class="`flex ml-auto text-white bg-${theme}-500 border-0 py-2 px-6 focus:outline-none hover:bg-${theme}-600 rounded`"
        >
          Button
        </button>
      </div>
    </div>
  </section>
</template>

<route lang="yaml">
meta:
  layout: empty
</route>

<style></style>
