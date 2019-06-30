<template>
  <Layout>
    <article class="max-w-xl pr-6">
      <section>
        <ul v-for="edge in $page.posts.edges" :key="edge.node.id">
          <li>
            <h2>{{ edge.node.title }}</h2>
          </li>
        </ul>
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
export default {
  metaInfo: {
    title: "Hello, world!"
  }
};
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
