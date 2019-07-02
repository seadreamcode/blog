<template>
  <aside class="mt-6 px-6 sm:max-w-xs sm:pb-6">
    <Header :title="$static.metaData.siteName" />
    <section>
      <section>
        <div class="my-6 text-xs">
          <div class="inline-block rounded-full py-1 px-4 mr-1 mb-2 bg-green-200">Node</div>
          <div class="inline-block rounded-full py-1 px-4 mr-1 mb-2 bg-blue-200">Golang</div>
          <div
            class="inline-block rounded-full py-1 px-4 mr-1 mb-2 bg-blue-800 text-white"
          >Typescript</div>
          <div class="inline-block rounded-full py-1 px-4 mr-1 mb-2 bg-yellow-200">Python 3</div>
          <div class="inline-block rounded-full py-1 px-4 mr-1 mb-2 bg-purple-200">PHP</div>
          <div class="inline-block rounded-full py-1 px-4 mr-1 mb-2 bg-blue-500 text-white">Docker</div>
        </div>
        <div class="mb-4">
          <span class="block underline">GitHub</span>
          <ul class="list-inside mb-2">
            <li>
              <a class="text-blue-700" href="#">seadreamcode</a>
            </li>
            <li>
              <a class="text-blue-700" href="#">chickencoder</a>
            </li>
          </ul>
        </div>
        <p class="mb-4">
          <span class="block underline">Twitter</span>
          <a class="text-blue-700" href="#">@jessethesibley</a>
        </p>
        <p class="">
          <span class="block underline">Email</span>
          <a class="text-blue-700" href="#">hi@seadream.dev</a>
        </p>
      </section>
    </section>
  </aside>
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

export default {
  components: {
    Header
  }
}
</script>