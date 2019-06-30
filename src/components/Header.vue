<template>
  <header class="max-w-4xl mx-auto p-6">
    <div class="flex sm:items-center flex-col sm:flex-row justify-between">
      <div class>
        <h1 class="font-semibold text-2xl">
          <g-link to="/">{{ title }}</g-link>
        </h1>
        <h2>
          Jesse Sibley's Blog
          <a
            class="text-blue-700 text-xs"
            href="https://github.com/seadreamcode/blog"
          >(View Source)</a>
        </h2>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  props: ['title']
}
</script>