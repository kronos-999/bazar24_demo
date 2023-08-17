<script setup lang="ts">
// https://github.com/vueuse/head
// you can use this to manipulate the document head in any components,
// they will be rendered correctly in the html results with vite-ssg
useHead({
  title: 'Bazar24',
  meta: [
    { name: 'description', content: 'The marketplace for you' },
    {
      name: 'theme-color',
      content: () => isDark.value ? '#172554' : '#ffffff',
    },
  ],
  link: [
    {
      rel: 'icon',
      type: 'image/svg+xml',
      href: () => preferredDark.value ? '/favicon-dark.svg' : '/favicon.svg',
    },
  ],
})
</script>

<template>
  <RouterView v-slot="{ Component }">
    <template v-if="Component">
      <Transition>
        <Suspense>
          <div>
            <!-- main content -->
            <component :is="Component" />
          </div>

          <template #fallback>
            <!-- loading state -->
            Loading...
          </template>
        </Suspense>
      </Transition>
    </template>
  </RouterView>
</template>

<style lang="postcss">
#nprogress .bar {
  @apply shadow-3xl shadow-white;
}
</style>
