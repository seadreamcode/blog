<template>
  <div class="layout container mx-auto">
    <div class="flex flex-col sm:flex-row">
      <Sidebar />
      <main class="mt-6 px-6 max-w-4xl">
        <slot />
      </main>
    </div>
  </div>
</template>

<script>
import Sidebar from '~/components/Sidebar'

export default {
  components: {
    Sidebar
  }
}
</script>

<style>
@tailwind base;
@tailwind components;
@tailwind utilities;

@media (min-width: 1024px) {
  .container {
    max-width: 1024px;
  }
}
</style>