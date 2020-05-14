<template>
<div class="container">
    <ul>
        <nuxt-link :to="`${blog.slug}`" v-for="blog in blogPosts" :key="blog.slug">{{blog.title}}</nuxt-link>
    </ul>
</div>
</template>

<script>
export default {
  computed: {
    blogPosts() {
      return this.$store.state.blogPosts;
    },
  },
  methods: {
      goToDetail(slug) {
          this.$router.push(`${slug}`)
      }
  }
}
</script>

<style>

</style>