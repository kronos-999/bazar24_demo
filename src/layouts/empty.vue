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
