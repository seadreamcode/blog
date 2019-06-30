<template>
  <div class="layout">
    <Header :title="$static.metaData.siteName" />
    <main class="max-w-4xl mx-auto px-6 flex flex-col sm:flex-row">
      <Sidebar />
      <slot />
    </main>
  </div>
</template>

<static-query>
query {
  metaData {
    siteName
  }
}
</static-query>

<script>
import Header from '~/components/Header'
import Sidebar from '~/components/Sidebar'

export default {
  components: {
    Header,
    Sidebar
  }
}
</script>

<style>
@tailwind base;
@tailwind components;
@tailwind utilities;
</style>