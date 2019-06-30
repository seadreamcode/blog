<template>
  <aside class="sm:max-w-xs sm:pb-6">
    <section>
      <article>
        <header>
          <div>
            <span class="block text-5xl" role="img" alt="Man Technologist Emoji">👨‍💻</span>
          </div>
          <p>
            <strong>Hello, I'm Jesse</strong>
          </p>
          <p class="my-2">19 years old &mdash; Junior Web Developer</p>
          <p class="mb-6">
            I'm interested in
            <mark class="bg-green-200 font-semi">Serverless</mark>,
            <mark class="bg-green-200">GraphQL</mark> &amp; the
            <mark class="bg-green-200">World Wide Web</mark>. I also make electronic instruments.
          </p>
        </header>
      </article>
      <section>
        <div class="mb-4 text-xs">
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
        <p class="mb-6">
          <span class="block underline">Email</span>
          <a class="text-blue-700" href="#">hi@seadream.dev</a>
        </p>
      </section>
    </section>
  </aside>
</template>

<style>
    @media (min-width: 640px) {
        .sm\:max-w-xs {
            max-width: 14rem !important;
        }
    }

    .\:max-w-xs {
        max-width: 14rem !important;
    }
</style>