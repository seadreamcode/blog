<template>
  <Layout>
    <article class="mb-6">
      <header>
          <div>
            <span class="block text-5xl" role="img" alt="Man Technologist Emoji">👨‍💻</span>
          </div>
          <article class="mb-4">
            <p>
              <strong>Hello, I'm Jesse</strong>
            </p>
            <p class="my-2">19 years old &mdash; Junior Web Developer <span class="bg-blue-200 p-1 rounded-sm text-xs">Devon, UK</span></p>
          </article>
        </header>
    </article>
    <article>
      <section class="mb-6">
        <h2 class="font-semibold text-2xl mb-4">About Me</h2>
        <p class="mb-4"><a class="text-blue-800" href="https://mycreativetype.com">mycreativetype.com</a> defines me as an <strong>‘Innovator’</strong></p>

        <p class="mb-4">I love building new things for the web and sharing them with people. My creative processes include
          writing music, giving saracstic speeches and attempting to turn every single one of my ideas into a startup.</p>
        <p class="mb-4">I also run a small business with a friend
          friend, where we’re building a fully serverless e-commerce PWA to sell hand made concrete planters.</p>

        <p class="mb-4">Sometimes I make tiny electronic instruments for fun.</p>
      </section>
      <section>
        <h2 class="font-semibold text-2xl mb-4">Posts</h2>
        <div v-for="edge in $page.posts.edges" :key="edge.node.id">
          <PostCard :post="edge.node" />
        </div>
      </section>
    </article>
  </Layout>
</template>

<page-query>
query Posts {
  posts: allPost {
    edges {
      node {
        id
        title
      }
    }
  }
}
</page-query>

<script>
import PostCard from '~/components/PostCard'

export default {
  metaInfo: {
    title: 'Blog'
  },
  components: {
    PostCard
  }
}
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
