<template>
  <Layout>

    <!-- Learn how to use images here: https://gridsome.org/docs/images -->
    <g-image alt="Example image" src="~/favicon.png" width="135" />

    <h1>this is a blog.</h1>

    <p>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Pariatur excepturi labore tempore expedita, et iste tenetur suscipit explicabo! Dolores, aperiam non officia eos quod asperiores
    </p>
    <h2>posts</h2>
    <p v-bind:key="post.title" v-for="post in $page.posts.edges">
      <g-link :to="post.node.path">
        {{ post.node.title }}
      </g-link>
    </p>

    <p class="home-links">
      <a href="https://gridsome.org/docs/" target="_blank" rel="noopener">Gridsome Docs</a>
      <a href="https://github.com/gridsome/gridsome" target="_blank" rel="noopener">GitHub</a>
    </p>

  </Layout>
</template>
<page-query>
query Posts {
  posts: allPost {
    edges {
      node {
        title
        path
      }
    }
  }
}
</page-query>

<script>
import { Pager } from 'gridsome'
export default {
  metaInfo: {
    title: 'Welcome'
  }
}
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
